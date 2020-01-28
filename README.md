# Team Hub

A configuration driven dev team dashboard that provides organized access to team resources and a comprehensive projects monitoring tool. team-hub-ui takes a JSON configuration object that drives all the functionality.

## To Run:

##### Prerequisites:
You must have **docker-compose**. If you don't have it, [install docker](https://docs.docker.com/get-started/).

If you have docker installed but don't have docker-compose, [install docker-compose](https://docs.docker.com/compose/install/)

#### Cloning the project & Setup:
After you clone the project prepare the submodules:
```bash
git clone https://github.com/dmhuebner/team-hub
cd team-hub

npm run prepare
```

#### Run the project:

Start up the project server and UI containers:
```bash
npm start
```

Stop the project server and UI containers:
```bash
npm run stop
```

### To Update Submodules:

```bash
npm run updateSubmodules
```

## Configuraiton
Team Hub is 100% configuration driven. This means all of the behavior of Team Hub can be customized for any Scrum Team.

The configuration object is located in the team-hub-ui project under team-hub-ui/src/assets/config.json.

The configuration object must match the TeamConfig TypeScript Interface below:

```
TODO
```

the team-hub-ui project has an example configuration object for your reference.

## Development

This project is made up of 2 git submodules: **team-hub-ui** and **team-hub-api**.

team-hub-ui is an Angular project that provides the configurable front end of Team Hub. The configuration JSON file is in team-hub-ui/src/assets/config.json.

team-hub-api is a Nest project that provides a websockets server that processes the configuration JSON object from the front end. It monitors the team projects (and any dependencies) as specified in the config file.

#### Contributing

Any code contributions to Team Hub should be made to the separate team-hub-ui or team-hub-api repos. The updateSubmodules npm command referenced above is available in this project to update the ui or server submodules with any new changes to those projects.

Run the following command to update the submodules in this team-hub project with any new changes.

`npm run updateSubmodules`

## TODO
