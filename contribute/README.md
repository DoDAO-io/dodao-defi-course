## Course Files
We add the files in yaml format. The reason we use YAML format is because it is easier to write a YAML as compared to JSON.
Also, YAML provides easy way to work with multi-line strings.

With-in the course YAML files, we have `content`, `details` or `summary` fields. These fields can contain multi-line strings. The
contents of these multi-line strings can be in Markdown format.

So the outer structure of the files are in YAML format, but `content`, `details` or `summary` fields are read and rendered as markdown content.

If you are willing to contribute, it is very important that you understand the basics of YAML and markdown format

## Learn YAML
You can go through these tutorials or watch any of the youtube videos on YAML

[https://www.cloudbees.com/blog/yaml-tutorial-everything-you-need-get-started](https://www.cloudbees.com/blog/yaml-tutorial-everything-you-need-get-started)

[https://www.tutorialspoint.com/yaml/index.htm](https://www.tutorialspoint.com/yaml/index.htm)

## Learn Markdown
You can go through these articles or watch any of the youtube videos on Markdown

[https://www.markdowntutorial.com/](https://www.markdowntutorial.com/)

## Setup
Use a proper IDE that can validate yaml file and also that shows markdown in view format.

## `src` folder
All our course files are present in the src folder. We read these files to generate course in markdown and in JSON
format.

## `course.yaml`
`course.yaml` is the main file that contains the course title, summary, description and details of all the chapters.

```yaml
title: DeFi 101 Course  # This is the title of the course
key: defi-course  # A unique key/identifier for the course
summary: This is a DeFi 101 Course # A multiline string that summarizes the course. This should be one paragraph about the course
details:  |   # A multiline string that captures the details of the course. This should be one page about the course
  Decentralised Finance (DeFi) is the upcoming revolution in the world which would result in 
  the complete transformation in the functioning of the finance sector using blockchain technology as its core.  
duration: 45 - 60 mins
topics:  # Topics field is an array/list field that consists of all the chapters of the course. 
  - title: What is DeFi and Use Cases # Title of the topic/chapter
    key: what-is-defi # A unique key/identifier for the topic/chapter
    details: | # A multiline string explaining every thing that is covered in this chapter
      This chapter explains basics of DeFi, How its different from Traditional Finance, and Use Cases
      
      Details
        * What is DeFi 
        * CeFi vs DeFi
        * Use cases of DeFi
    readings: blockchain_basics.yaml # name of the file in `src/readings` folder that corresponds to the readings for this chapter
    summaries: blockchain_basics.yaml # name of the file in `src/summaries` folder that corresponds to the summaries for this chapter
    questions: blockchain_basics.yaml # name of the file in `src/summaries` folder that corresponds to the questions for this chapter
    status: In Progress # Status -> Not Started, In Progress, or Completed
    completionWeek:  July 18 # In which week can we expect this chapter to be completed
```

## Summaries file
This is a list of sub-topics in a chapter which we will summarize. Intent is that the user can revise each and every concept
in the chapter by going through the bullet points. Please look at "Two Minute Drill" sections in SCJP
book ([https://firozstar.tripod.com/_darksiderg.pdf](https://firozstar.tripod.com/_darksiderg.pdf))

```yaml
- title: Value Types # Title of the Sub Topic
  shortTitle: Value Types # A short title which is shown in left nav bar on the UI
  key: value-types # A unique key/identifier for the course
  details: | # details is the bullet points which summarize the Sub Topic. It is a multi-line string in Markdown format
    The following types are called value types because variables of these types will always be passed by value, i.e. unlike reference types they are always copied when used in function arguments or asssignments.
    - Booleans
      * They are declared using the keyword `bool`.
      * The possible values are constants true and false.

    - Integers
      * They are declared using keywords `int` , `uint` for signed and unsigned integers.
      * Keywords `uint8` to `uint256` in steps of 8 are used to store unsigned integers with varying sizes in bits. Similarly , `int8` to `int256` for signed integers.
      * For Example, uint32 is a 32 bit unsigned integer having range from 0 to $2^{32}-1$ whearas int32 is a 32 bit signed integer having range from $-2^{31}$ to $2^{31}-1$.
      * For an integer type X, you can use `type(X).min` and `type(X).max` to access the minimum and maximum value representable by the type.
      * Integers allow the use of comparision (<=, <, ==, !=, >=, >) , bit (&, |, ^ , ~) , arithmetic (+, -, *, /, %, ** ) and shift (<< , >>) operators.
      * `x << y` is equivalent to the mathematical expression $x * 2^y$. `x >> y` is equivalent to the mathematical expression $x / 2^y$.

```

## Readings File
We refer to Youtube video or an Article/Link as reading. Reading file consist of list of readings.

Each reading is represented in the following format

```yaml
- uuid: a150cd2d-1888-4210-8bee-9411eb25e3bf # uuid Needs to be a random UUID - You can generate it from https://www.uuidgenerator.net/version4.  Use version 4
  title: Introduction to Solidity Data types # Title of the video. This doesn't need to match the youtube video title
  shortTitle: Data Types Intro - 1 # A short title which is shown in left nav bar on the UI
  type: YoutubeVideo # Type can be YoutubeVideo or Article
  url: https://www.youtube.com/watch?v=N1Jeeei_wtw  # URL of the video or article
  subTopics:  # List of sub-topics from summaries about which this video is
    - "value-types"
    - "reference-types"
    - "mapping-type"
  details: | # Here we share in our own words what this video is all about
    In this video we're looking at the data types available in Solidity.
    This video explains about the use of -
    * Value Types - Integers , Booleans etc 
    * Reference Types - Structs , Arrays .
    * Mapping Type - Mapping.
```

## Questions
Questions should be written in the following format

Wrap the content with ``` (three backticks) if you are writing a multiline code string

Wrap the content with ` (single backtick) if you are writing some single line keyword or code
```yaml
- uuid: a2bc4929-787b-4184-959c-480659493663
  type: SingleChoice # Types can be MultipleChoice or SingleChoice
  content: | # Content should be in Markdown format. Can be a multiline string
    In the following code snippet which line will result in an error-
      ```
      // SPDX-License-Identifier: MIT
      pragma solidity ^0.8.10;
      contract C {

          //line 1
          uint public x = 1;

          // line 2
          function addToX(uint y) public pure returns (uint) {
              return x + y;
          }

          // line 3
          function add(uint i, uint j) public pure returns (uint) {
              return i + j;
          }
      }
    ```
  hint: Check whether the function declaration is correct. # Hint for the user. Use NoHint "only" if you feel the question is too simple
  explanation: | 
    Pure declares that no state variable will be changed or read in a function. view tells us that by running the 
    function, no data will be saved/changed. Here in line 2 a pure function is trying to read the data from a state 
    variable. The declaration should have a view instead of pure.
  answerKeys:
    - B
  subTopics: # List of sub-topics from summaries about which this video is
    - "value-types"
  difficultyLevel: Low # Difficulty level should be one option from "Low" , "Medium", "High"
  choices:
    - content: Line 1 # Content should be in Markdown format
      key: A
    - content: Line 2
      key: B
    - content: Line 3
      key: C
    - content: The code snippet will not give any error
      key: D
```

## Validation

Run `yarn test` in the course folder to see if the changes you have done are correct.

Also check the generated markdown format in the view format.

## commit

Create a new branch in the same main repository and create a pull request.
