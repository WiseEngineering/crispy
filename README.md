# crispy
Docs/Links/Infrastructure. Successor to database management tools

## Overview 

This is a tool to make developers life easier and database setup more reliable.

## Architecture

### Components

#### crispy 

  - https://github.com/WiseEngineering/crispy-worker
  - https://github.com/WiseEngineering/crispy-web
  - https://github.com/WiseEngineering/crispy-api

They must manage all database operations and be able to execute them in a particular worker. 
The main goal for those Components to be responsible for running database operations in `worker` and give the user the ability to manage it from [WEB](https://github.com/WiseEngineering/crispy-web)

#### crispy-toolkit

https://github.com/WiseEngineering/crispy-toolkit

Simple CLI interface where you are able to sync your migrations with `crispy` Component.

## How components will interact with each other

- [crispy-web](https://github.com/WiseEngineering/crispy-web) communicates with [crispy-api](https://github.com/WiseEngineering/crispy-api)

 - [crispy-web](https://github.com/WiseEngineering/crispy-web) communicates with [crispy-worker](https://github.com/WiseEngineering/crispy-worker)
 
- [crispy-toolkit](https://github.com/WiseEngineering/crispy-toolkit) communicates with migrations folder/library based on adapter

- [crispy-toolkit](https://github.com/WiseEngineering/crispy-toolkit) communicates with [crispy-api](https://github.com/WiseEngineering/crispy-api)


