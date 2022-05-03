---
marp: true
---
## Team 28: Classroom setting Discord server + Migration
### By: Cade Cofer, James Norum, Saadman Shan, Cin Vaan
---
## Table of contents
- Introduction to the problem
- Approaches to the solution
- Issues/Conflicts faced
- Approaches to resolving issues/conflicts
- Implementation
- Demo
- References
---
## Introduction to the problem
- The ask:
    - "Classroom setting Discord server + Migration"
- Our interpretation of the ask: 
    - Create a discord server with classroom settings and capabilities, and include a migration from another server to the newly created sever, or vice-versa.
---
## Approaches to the solution (Pt.1)
- Initial approach (scrapped)
    - Create test servers with minimal classroom setting, and code a bot in Python to assist in classroom settings. Migration was approached as a functionality for the developed bot
- Second approach (scrapped)
    - Create a test server using "SayYes" Discord server as a reference, and code multiple bots in multiple languages to assist in classroom settings. Migration was approached as a functionality for the developed bots.
---
## Approaches to the solution (Pt.2)
- Final Approach
    - Create a test server using "SayYes" and "OUCS" Discord servers as a reference, utilize a pre-built bot to assist in classroom functions within the server, and develop a bot in Python that handles migration.
---
## Issues/Conflicts faced
- Understanding the problem
    - Vagueness of requirements
    - Insufficient understanding of Discord and Discord's API
    - Insufficient understanding of Python and JavaScript
- Researching solutions
    - Minimal resources found on assisting in migration
    - Some pre-built bots require a paid subscription/have limited functionalities
- Team issues/conflicts
    - Proper scheduling of tasks
    - Improper division of responsibilities amongst team members
---
## Approaches to resolving issues/conflicts (Pt.1)
- Understanding the problem
    - Vagueness of requirements
        - Assumed to be so in order for teams to create their own scope of requirements
        - Requirements were assessed by the Team to curate the above assumtion of the problem and the proposed approach to the solution
    - Insufficient understanding of Discord and Discord's API
        - Research was required
        - Team members created their own "sand-box" servers to familiarize themselves with Discord and its API.
    - Insufficient understanding of Python and JavaScript
        - Research was required
        - "Sand-box" servers were used to learn, practice, and test features of "sand-box" bots created using Python and JavaScript.
---
## Approaches to resolving issues/conflicts (Pt.2)
- Researching solutions
    - Minimal resources found on assisting in migration
        - Discord does not allow for user migrations without user input, even through the use of bots.
        - Created a bot that asks for user input in order to migrate users
        - Messages and other content posted will not be migrated
    - Some pre-built bots require a paid subscription/have limited functionalities
        - Research was required
        - Multiple pre-built bots were tested in "sand-box" servers for various functionalities
        - Atlas bot was used in the final implementation
---
## Approaches to resolving issues/conflicts (Pt.3)
- Team issues/conflicts
    - Proper scheduling of tasks
        - Multiple restructurings of workflow
        - Meet at least once a week to reasses workflow and tasks
    - Improper division of responsibilities amongst team members
        - Multiple meetings to reasses responsibilities of individual team members
        - Discourse throughout the semester on how to share responsibilities better
        - Divided tasks and responsibilities based on individual strengths and weaknesses
---
## Implementation (Pt.1)
- Create Server using "SayYes" and "OUCS" Discord servers as a reference
    - 1 server
        - "Events" channel for events to be posted by moderator
        - "rules" channel to display rules for the server and for users to select their role
        - "moderator-only" channel to display the activity on the server for moderators
        - "general" channel for general discussions on the server
        - 28 hidden folders correlating to 28 OU Computer Science courses
        - 28 user roles correlating to the 28 folders created
        - Folder(s) opens for user based on their selected role
---
## Implementation (Pt.2)
- Create Server using "SayYes" and "OUCS" Discord servers as a reference (cont.)
    - 28 hidden folders
        - Each contains channels that can only be accessed if the user has the role to access the folder
        - "announcements" channel for moderators to post announcements for the class
        - "general" channel for general discussions for the class
        - "discussions" channel for voice-discussions for the class
---
## Implementation (Pt.3)
- Pre-built bot (Atlas)
    - Atlas
        - Creates a "Reaction Roles" message in "rules" channel of the server
        - Sends a PM to a user when they first join the server on directions on how to use the server
        - Users react to the message by clicking the button for the role(class) they want to have
        - Atlas assigns role to the user based on their selection
        - The server opens up folders based on their role
---
## Implementation (Pt.4)
- Bot built using python
    - Sends a message to all channels in a server that the bot is in
    - Message contains an invite link to our built server
    - This is a user-approved migration
---