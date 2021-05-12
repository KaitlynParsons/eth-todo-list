# Ethereum Blockchain Todo List
End to end tutorial writing a todo list app on the ethereum blockchain.
[Link to Tutorial](https://youtu.be/coQ5dg8wM2o)

## Requirements
- Ganache
- NodeJS
- truffle 5.0.2 (npm install -g truffle@5.0.2)
- Metamask

## Setup
- Create new workspace in Ganache
- Run truffle init 
  - ### Contract
    - Create your contract file under contracts and include all logic
    - Create your migration js file under migrations to deploy it to your blockchain instance
    - Run truffle migrate

## Helpful Notes
- Checking TodoList contract in the truffle console:
  - truffle console
  - todoList = await TodoList.deployed()
  - todoList.address
  - taskCount = await todoList.taskCount()
  - taskCount.toNumber()
