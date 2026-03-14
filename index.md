---
waltz:
  title: EGDD - RushAPI
meta:
  version: 0.0.1
  gdd authors:
    - Bruce Bermel <brbe@udel.edu>
    - John-Paul Newton <jpnewton@udel.edu>
  template authors:
    - Austin Cory Bart <acbart@udel.edu>
    - Mark Sheriff
    - Alec Markarian
    - Benjamin Stanley
---


# RushAPI

## Elevator Pitch

You are an API service that is responsible for handling user's requests. The goal is to complete these requests by writing proper API requests in a given amount of time and responding properly. The difficulty of the game comes in more endpoints being added and requests coming in more rapidly

## Influences (Brief)

- Overcooked:
  - Medium: *Game*
  - Explanation: I think the idea of a fast-paced "response to orders" style game fits the structure of API requests perfectly. I also think the idea of knowing what request to write should be second nature, so rapidly repeating this process build good habit
- Mini Motorways:
  - Medium: *Game*
  - Explanation: The simple and addicting aesthetic makes playing the game feel natural and reptitively fun
- Postman:
  - Medium: *Utility*
  - Explanation: Most accurately mirrors the actions of the user

## Core Gameplay Mechanics (Brief)

*Give a very high-level description of any core gameplay mechanics*

- Users with pre-set ID numbers (on shirt) make requests
- User decides what type of request and accesses "database"
- Depending on request type, user performs proper operation
- User selects proper response code to give back
- Timeout bar that can be replenished via dollars, however only a set number of dollars ever exist
- Game over when timeout
- Users can have "special requests" that give certain powerups when completed
- As game progresses, timeout speeds up and schema grows new tables

# Learning Aspects

## Learning Domains

- Database management
- API Request Types
- Handling API Request Responses
- JSON Handling


## Target Audiences

Sophomore/Junior Undergraduate CS Students

## Target Contexts

Supplementary practice for an assignment that introduces uses API calls without directly teaching them

## Learning Objectives

*Remember, Learning Objectives are NOT simply topics. They are statements of observable behavior that a learner can do after the learning experience. You cannot observe someone "understanding" or "knowing" something.*

- Recognize API Requests*: After playing, students will be able to identify the proper API request type for a given use case
- Handle Response: After playing, students will be able to selecting the proper respsonse code for different API request scenarios
- JSON Handling: After playing, students should be able to construct proper json content for API requests
- JSON Parsing: After playing, students should be able to identify key fields in API JSON response

## Prerequisite Knowledge

*What do they need to know prior to trying this game?*

- Players should be able to identify the purpose of API Requests
- Players should be able to connect the use of API requests to databases
- Players should be able to roughly identify entity relationships in databases

## Assessment Measures

Given a list of API use cases, identify the correct API request type to use
Given an API Response code, identify its meaning
Given an item and its description, create a JSON object to represent the item with all appropriate properties
Given a JSON response and a key, identify the value associated with the key



# What sets this project apart?

*Give some reasons why this game is not like every other game out there. Whether the learning objective is unique, the gameplay mechanics are new, or what. You should persuade the reader that your game is novel and worthy of development. Consider arguments that would be persuasive to a Venture Capitalist, Teacher, or Researcher. These might be focused on learning needs, too.*

- The Game is made to teach the process of API requests, which is not something that is commonly taught well or at all
- The game is made to be addicting and mindless, to simulate a developer's actions when creating API requests
- The top-down/resource management genre of game is one that does not have a lot of competitors, making it a unique experience
- *COME BACK TO HERE*
- *Reason #4*
- *etc.*

# Player Interaction Patterns and Modes

## Player Interaction Pattern

This is a single-player game where the player interacts with the system by typing API requests into a text field and submitting them.

## Player Modes

-Endless Mode: The player continuously processes incoming user API requests, gaining additional time for each successful request, and the game ends when the timer runs out.

# Gameplay Objectives

- Complete API Requests:
    - Description: Players must construct correct API requests to satisfy NPC user requests.
    - Alignment: Reinforces learning of HTTP methods and endpoint structure.
- Respond Before Time Runs Out:
    - Description: The player must complete requests quickly in order to keep the timer from reaching zero. Each successful request adds additional time.
    - Alignment: Encourages rapid recognition of request patterns and reinforces repeated practice with API syntax.
- Construct Valid JSON Bodies:
    - Description: For certain requests such as POST, PUT, and PATCH, the player must correctly construct a JSON body containing the appropriate fields and values.
    - Alignment: Reinforces understanding of request payload structure.

# Procedures/Actions

Players can:
  - Select an NPC request from the queue
  - Type an API request
  - Enter a JSON body
  - Submit the request
  - View the simulated server response

# Rules

- Requests must be complete before the timer expires
- Correct requests will award points and time increase
- Incorrct requests will award no points and waste time
- Completing "boss" request grants temporary power-ups such as time slow/freeze or double points

# Objects/Entities

- NPC users requesting API operations
- "Boss" NPC requesting API operations with higher difficulty and rewards
- Request queue which displays incoming user requests
- Terminal where the player types the request
- JSON body input where the player
- Response window displays the server's response after the submitted request

## Core Gameplay Mechanics (Detailed)

- NPCs enter a queue requesting API actions. The player can select one of the top requests and must complete it before the timer runs out. If the the player takes too long to fulfill requests the timer will run out and the player will lose.
- Players must type the correct request in a curl style format. For certain requests, players must also provide a JSON body.
- After submitting a request, the system returns a simulated API response showing either success or an error.
    
## Feedback

- 202 Accepted: Displayed when the player submits a correct API request. The response window shows a success message, the player earns points, and additional time is added to the timer.
- 404 Not Found: Displayed when the player types an incorrect endpoint that does not exist in the API.
- 400 Bad Request: Displayed when the player submits an invalid or incorrectly formatted JSON body.
- 500 Internal Server Error: Displayed when the game ends because the timer runs out, indicating that the API server has become overloaded and can no longer process requests.
- Long-Term Feedback: The player’s score, time remaining, and total successful requests indicate how well they are performing over time.
- Difficulty: As the player progresses, requests become more complex with additional endpoints and JSON body requirements, helping players track their improvement.

# Story and Gameplay

## Presentation of Rules

*Briefly describe how the player will learn the gameplay mechanics. Avoid using walls of text, since people will not read them. Think instead of natural ways of teaching mechanics iteratively and slowly.*

## Presentation of Content

*Briefly describe how the player will be taught the core material they are meant to learn. Avoid using walls of text, since people will not read them. Think instead of natural ways of teaching material iteratively and slowly.*

## Story (Brief)

*The Summary or TL;DR version of below*

## Storyboarding

*Go into as much detail as needs be to visually convey the Dynamics of your game. Be detailed. Create storyboards and freeze frame images that concisely capture important key elements of your game. You are strongly recommended to sketch pictures on paper and embed them here. Be sure make it clear how previously-described mechanics come through in the dynamics.*

# Assets Needed

## Aethestics

*Give a sense of the aesthetics of your game, the spirit and atmosphere. Use descriptive, evocative words that can help the reader understand the emotional response of your game.*

## Graphical

- Characters List
  - *Characters 1*
  - *Characters 2*
  - *...*
- Textures:
  - *Texture 1*
  - *Texture 2*
  - *...*
- Environment Art/Textures:
  - *Environment Texture 1*
  - *Environment Texture 2*
  - *...*


## Audio


*Game region/phase/time are ways of designating a particularly important place in the game.*

- Music List (Ambient sound)
  - *Game region/phase/time*: *Example 1*, *Example 2*
  - *Game region/phase/time*: *Example 3*, *Example 4*
  
*Game Interactions are things that trigger SFX, like character movement, hitting a spiky enemy, collecting a coin.*

- Sound List (SFX)
  - *Game Interaction*: *Example 1*, *Example 2*
  - *Game Interaction*: *Example 3*, *Example 4*


# Metadata

* Template created by Austin Cory Bart <acbart@udel.edu>, Mark Sheriff, Alec Markarian, and Benjamin Stanley.
* Version 0.0.3
