# Adding Questions

Questions should be written in the following format
```yaml
# uuid Needs to be a random UUID - You can generate it from https://www.uuidgenerator.net/version4.  Use version 4
uuid: 1b8fbe3c-aeb2-4b7d-a3ef-3082bf07efcc
# Types can be MultipleChoice or SingleChoice
type: MultipleChoice
content: What does SW DAO offer?
answerKeys:
- e0kl
# should be from one of the predefined list of topics  
topic: "01_data_types"
# should be from one of the predefined list of sub-topics, or can be a new one  
sub_topics:
- "string"
- "variables"
# Difficulty level should be one option from "Low" , "Medium", "High"  
diffculty_level: "Low"
choices:
- content: It offers crypto based mining applications for effective utilization
    of resources.
  key: rtte
  order: 0
- content: It offers strategic DeFi investment products which allocate capital
    based on Machine Learning
  key: e0kl
  order: 1
- content: It offers coding and machine learning solutions to develop Defi
    applications.
  key: fklo
  order: 2
- content: All of the about options
  key: pwlp
  order: 3
  

```
