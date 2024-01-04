# Retrieval Augmented System for Research | ATP team | Department of Human Services

### Note: Due to the sensitive information contained in the source files, this repository has been made private. To review the implementation, please refer to this [open-source repository.](https://github.com/shayanalis/Retrieval-Augmented-Generation-for-Product-Management)

## Purpose
The tool assists Data Science, ML, and Econometrics researchers at DHS in swiftly searching curated material on topics such as:
This tool is used to help Data Science, ML, and Econometrics researchers at DHS to quickly search for curated material on topics like:
1. Modelling for County residents
2. Documented Best Practices
3. Vetted Research in DHS
4. Specific Table Lookups

## How to use
Open the deployed link and put in a question like:

1. "What are the best practices for handling years in my model"
2. "Which features should I use when modeling for ..."
3. "Research on maternal health outcomes in Allegheny County"

## How it works
The system uses an Agent to decide what information to search for, thinking at each step what is needed to answer the query. For example:


User: "What are the best practices for handling years in my model"

--> Invoking Agent-based Retrieval
> Agent: Thinking: I need to search for 'best practices in models'

> Agent: Thinking: I need to search for 'handling years in models'

--> Retrieval from vector store. 
--> Agent: Aggregating: Based on the information I need to search for 'Bad Examples of Modeling'

> Agent: Thinking: Using all the information to answer the user's question.

Assistant: "Here are the best practices... [reference: abc_health_outcomes.pdf] [reference: xyz_modelling.pdf]"
