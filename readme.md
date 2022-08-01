# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

**Cloning Anythink Market repo**

Clone Anythink Market repository locally using the following ([link](https://github.com/ObelusFamily/Anythink-Market-bt3f1.git)).

If you are facing any difficulty in cloning this repository, you can refer ([this](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)).

**Setting up the Enviornment**

After Cloning the repo, the next step is to setup the working environment, so that things would function smoothly on your local machine.

*Step1 - Install Docker*

You can install docker from the following ([link](https://docs.docker.com/get-docker/)).

You can verify docker is ready by running the following commands in your terminal: 
    docker -v
    
    docker-compose -v

*Step2 - Load Backend and Frontend*

After successfully installing docker, run the following command from the project root directory to load Anythink's backend and frontend.
    
    docker-compose up 

If Docker is working correctly, the backend should be running and able to connect to your local database.

*Step3 - Verifying Backend and Frontend*

Test the backend is functioning by clicking on this ([link] (http://localhost:3000/api/ping)).

Test the frontend is functioning by clicking on this ([link] (http://localhost:3001/register)) and create account by filling in all the input credentials.

Just make sure that you run all scripts on one of the containers created by docker-compose up. Also, you can use docker exec to run commands on a running container.
