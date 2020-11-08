# fullstack-graphql-airbnb-clone

A Fullstack GraphQL Airbnb Clone with React and React Native.

- Branches are in the order they were coded.
- Watch how this was made: https://www.youtube.com/playlist?list=PLN3n1USn4xlnfJIQBa6bBjjiECnk6zL6s
- This builds off the GraphQL Typescript Server I made: https://github.com/benawad/graphql-ts-server-boilerplate.
- You can see the YouTube Playlist for how that was made here: https://www.youtube.com/playlist?list=PLN3n1USn4xlky9uj6wOhfsPez7KZOqm2V
- Join the Discord: https://discord.gg/Vehs99V

## Packages

This project is made up of 5 packages that share code using Yarn Workspaces.

- web (React.js website)
- app (React Native app)
- server (GraphQL Typescript server)
- common (Code shared between web, app, and server)
- controller (Components shared between web and app)

## Installation

1. Clone project

```
git clone https://github.com/benawad/fullstack-graphql-airbnb-clone.git
```

2. cd into folder

```
cd fullstack-graphql-airbnb-clone
```

3. Download dependencies

```
yarn
```

4. Start the postgre server and the redis server

```
docker-compose up
```

5. The default username/password `postgres` could be changed in docker-compose.yml and ormconfig.json

6. Connect to the database with `psql` and add the uuid extension:

```
CREATE EXTENSION IF NOT EXISTS "uuid-ossp";
``` 

7. In `packages/server` create a file called `.env` and add the following line inside: `FRONTEND_HOST=http://localhost:3000`

8. Run `yarn build` in `packages/common`

9. Run `yarn build` in `packages/controller`

10. Get Google Maps API key and put it here index.html
More infos [here](https://developers.google.com/maps/documentation/javascript/get-api-key?utm_source=google&utm_medium=cpc&utm_campaign=FY20-Q3-global-demandgen-displayonnetworkhouseads-cs-GMP_maps_contactsal_saf_v2&utm_content=text-ad-none-none-DEV_c-CRE_321592199421-ADGP_Hybrid%20%7C%20AW%20SEM%20%7C%20BKWS%20~%20Google%20Maps%20API%20Key%20EXA-KWID_43700039907225615-kwd-2615963921-userloc_9055225&utm_term=KW_google%20maps%20api%20key-ST_google%20maps%20api%20key&gclid=Cj0KCQiAy579BRCPARIsAB6QoIaBzZVrdbVHPoC-B_-W_1mP5q25KQN_ya63JwM-n5OVSFdXplbi8nwaAo0UEALw_wcB)
Go to [Maps JavaScript API](https://console.cloud.google.com/apis/library/maps-backend.googleapis.com?q=Google%20Maps%20JavaScript%20API&id=fd73ab50-9916-4cde-a0f6-dc8be0a0d425&project=windy-furnace-180806) and click on 'Enable' to add 'Google Maps' to your projects.


## Usage

1. Start server `yarn start` in `packages/server`

2. Now you can run `yarn start` in `packages/web` or `packages/app` to start the website or app.

3. How to get credentials working in graphql playground: https://youtu.be/oM-EmNdhwI4?t=8m39s

## Deploy

### Server

1. https://www.youtube.com/watch?v=qQAozc1MkdU
2. https://www.youtube.com/watch?v=0t-rE5wUP-E

### Website

1. https://www.youtube.com/watch?v=FiU3SHEaFwk
2. https://www.youtube.com/watch?v=vPu1sfuYFzw
3. https://www.youtube.com/watch?v=Ry6Zobb-kaw

## Features

1. Website register/login
2. Deploy backend and frontend
3. App register/login
4. Website and App forgot password
5. Website and App create listing
6. Website and App view listings
7. logout
8. Website chat
