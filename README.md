# Ethereum Blockchain Todo List
- End to end tutorial writing a todo list app on the ethereum blockchain.
- [Link to Tutorial](https://youtu.be/coQ5dg8wM2o)

## Requirements
- Ganache
- NodeJS
- truffle 5.0.2 (npm install -g truffle@5.0.2)
- Metamask
- Metamask Legacy Web3

## Setup
- Create new workspace in Ganache 
  - ### Contract
    - Create your contract file under contracts and include all logic
    - Create your migration js file under migrations to deploy it to your blockchain instance
    - Run truffle migrate (use --reset flag to deploy a new copy)
- npm run dev

## Helpful Notes
- Running truffle init generates a new truffle project.
- Running truffle compile re-generates the contracts for the build.
- Checking TodoList contract in the truffle console:
  - truffle console
  - todoList = await TodoList.deployed()
  - todoList.address
  - taskCount = await todoList.taskCount()
  - taskCount.toNumber()
- Listing out tasks in the TodoList:
  - todoList = await TodoList.deployed()
  - task = await todoList.tasks(1)
  - task
