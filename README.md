# Team Hub

## To Run:

##### Prerequisites:
You must have **docker-compose**. If you don't have it, [install docker](https://docs.docker.com/get-started/).

If you have docker installed but don't have docker-compose, [install docker-compose](https://docs.docker.com/compose/install/)

#### Cloning the project:
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
