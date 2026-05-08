# GP25 AI Programming Assignment

## Overview
TODO:
- What the project goal is
- What the project contains (RED and GREEN NPCs)
- Tools used (engine, template, base classes & source control)

## Content Folder Structure
```
Content/
|--Assignment/
|  |--NPC_00 (the RED guy)
|  |  |--BP_NPC_00_Character (character blueprint)
|  |  |--BP_NPC_00_Controller (AI controller blueprint)
|  |  |--BehaviorTree
|  |  |  |--BB_NPC_00_Blackboard
|  |  |  |--BT_NPC_00_BehaviorTree
|  |  |  |--(BT tasks & services blueprints)
|  |--NPC_01 (the GREEN guy)
|  |  |--BP_NPC_01_Character (character blueprint)
|  |  |--BP_NPC_01_Controller (AI controller blueprint)
|  |  |--BehaviorTree
|  |  |  |--BB_NPC_01_Blackboard
|  |  |  |--BT_NPC_01_BehaviorTree
|  |  |  |--(BT tasks & services blueprints)
|
(Template-provided folders & content)
|--Characters...
|--Cursor...
|--LevelPrototyping...
|--TopDown...

```

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