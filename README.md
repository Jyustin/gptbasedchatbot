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

3: configure backend as needed

4: add cc-assistant.html (the frontend of the bot) and the assets folder to your frontend repository, configuring paths and the header of the html file to match up with your project. any frontend should work, however this project was built on this one: https://github.com/nighthawkcoders/Nighthawk-Pages

5: run both backend and frontend locally and test endpoints as well as frontend and backend connectivity

