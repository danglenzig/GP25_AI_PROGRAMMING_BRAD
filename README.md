# GP25 AI Programming Assignment

## Overview
TODO:
- What the project goal is
- What the project contains (RED and GREEN NPCs)
- Tools used (engine, template, base classes & source control)

## Content Folder Structure
...

## NPC Implementation
```mermaid
flowchart TD
    CHAR[NPC Character]
    CONT[NPC AI Controller]
    BLAK[Blackboard]
    TREE[Behavior Tree]
    TASK[BT Tasks]
    SRVC[BT Services]
    CHAR -->|Controlled by| CONT
    CONT -->|Runs| TREE
    TREE -->|Reads data from| BLAK
    TREE -->|Implements| TASK
    TREE -->|Implements| SRVC
    TASK -->|Reads & writes data to| BLAK
    SRVC -->|Writes data to| BLAK
```

TODO: discuss...
* Character BP
* Controller BP
* Blackboard
* Behavior Tree
* Behavior Tree Tasks
* Behavior Tree Services