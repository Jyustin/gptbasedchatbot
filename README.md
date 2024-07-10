this repository contains parts for a chatgpt based chatbot project

view the chatbot here: https://codemaxxers.github.io/codemaxxerFrontend/bot (NOT WORKING AT MOMENT)

original frontend: https://github.com/Codemaxxers/codemaxxerFrontend

original backend: https://github.com/Codemaxxers/codemaxxerBackend

NOTE: this is mostly guidelines to help with building the project, not so much instructions. Do not expect this to work out of the box, some configuration will have to be done.

## CONTENTS:

assets: contains files neccessary for frontend to run

cc-assistant.html: the front page for the bot

chathistory: contains java files meant to work with a spring backend. This was tested on a spring_portfolio template mentioned below.

# HOW TO USE:

1: create a new repository using this github template: https://github.com/nighthawkcoders/spring_portfolio

this is a java backend built on spring, and will be used for the endpoints for our project

2: open the new backend repository and place the chathistory folder into the following directory
YOURBackend\src\main\java\com\nighthawk\spring_portfolio\mvc

3: add your own api key variables to .env (see guide below for obtaining all the necessary variables)

4: add cc-assistant.html (the frontend of the bot) and the assets folder to your frontend repository, configuring paths and the header of the html file to match up with your project. any frontend should work, however this project was built on this one: https://github.com/nighthawkcoders/Nighthawk-Pages

5: run both backend and frontend locally and test endpoints as well as frontend and backend connectivity

### obtaining api variables from OPENAI

This part of the guide will be a walkthrough to acquiring the assistantId, threadId, and aiKey, which are required for accessing the OPENAI api.

1. go to https://platform.openai.com/account/api-keys and create an account or log in

2. create a new secret key, with all permissions, and save your key. Add the secret to the .env for the ai_key variable.

3. click on Assistants on the left navbar and create a new assistant. Take note of the assistant id at the top, as this is the assistant id. add that id variable to your .env for the ai_asst_id variable.

4. afterwards, click on the Assistants from the Playground section of the left navbar, and send a message.

5. copy the thread id generated from the message and add it to the .env for the ai_thread_id variable.

IMPORTANT: It is important to hide your secret variables to prevent theft of keys. Do not commit the .env with all of the variables within directly to github, as your key will likely get stolen. There are many different solutions for hiding secrets, however the one I used was simply splitting each variable into 2 separate strings, then concatenating them when I needed those secret variables.


