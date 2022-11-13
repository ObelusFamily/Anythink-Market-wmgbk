# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

**[TODO 05/01/2018 @vanessa-cooper]:** _It's been a while since anyone ran a fresh copy of this repo. I think it's worth documenting the steps needed to install and run the repo on a new machine?

1. Clone code from GitHub here,[Anythink-Market-wmgbk](https://github.com/ObelusFamily/Anythink-Market-wmgbk.git)
2. [Install Docker](https://docs.docker.com/get-docker/)
3. Update Dockerfile within backend -> scripts to use python version 3.9.12 and then remove poetry version (==1.1).
3. Run the command `'docker-compose up --build'` from the project root directory.
    - you can use `'docker exec'` to run commands on a running container.
4. Test start up, [ping local site](http://localhost:3000/api/ping)
5. Create new user at [register screen](http://localhost:3001/register)