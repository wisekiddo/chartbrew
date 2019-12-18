<p align="center">
  <a href="https://chartbrew.com">
    <img src="https://docs.chartbrew.com/assets/cb_logo_4.png" alt="ChartBrew logo" width="250"/>
  </a>
</a>

<p align="center">
  <a href="https:/\/circleci.com/gh/razvanilin/chartbrew">
    <img src="https://circleci.com/gh/chartbrew/chartbrew.svg?style=svg" alt="ChartBrew build" />
  </a>
</p>

[ChartBrew](https://chartbrew.com) is an open-source web application used to generate charts from different data sources. The focus of this project is to make the process less tedious and put as much accent as possible on Usability.

This project was created by [Kate Belakova](https://github.com/belakova) and [Razvan Ilin](https://github.com/razvanilin)

📚 [**Read the full docs here**](https://docs.chartbrew.com)

🔧 [**Development roadmap**](https://github.com/orgs/chartbrew/projects/1) - start here if you want to contribute

🚙 [**Public feature roadmap over here**](https://trello.com/b/IQ7eiDqZ/chartbrew-roadmap)

💬 [**Join our Slack workspace**](https://join.slack.com/t/chartbrew/shared_invite/enQtODU3MzYzNTkwOTMwLTZiOTA5YzczODUzZGFiZmQyMGI1ZGVmZGI4YTVmOTBkMTI0YzQ2ZjJjOGI5NzQ0NmNmYzRmMDk3MmY4YmI4MTI)

## Data sources

Currently, ChartBrew supports connections to these data sources.

* MySQL
* PostgreSQL
* MongoDB
* APIs that support JSON data

## Prerequisites

* NodeJS v10.16.0+
* NPM
* MySQL v5+ Server running

## Quickstart

**Create a new database** that you're going to use with Chartbrew. Also, note down the username and password because you will need them in the next steps.

```sh
npx create-chartbrew-app myApp --dbname="chartbrew" --dbusername="root" --dbpassword="" --dbhost="localhost"
```

The arguments are optional, but they set the environmental variables needed for the project to run. [Check out which need to be set here.](https://docs.chartbrew.com/#set-up-environmental-variables)

**Run the database migrations**

Ensure all the environmental variables are set, then run the following command in the `server` folder:

```sh
npm run db:migrate
```

### Run the project in Development

Open two terminals, one for front-end and the other for back-end.

```sh
# frontend
cd client/
npm run start

# backend
cd server/
npm run start-dev
```

For more information on how to configure, modify and deploy ChartBrew, [**read the full docs here**](https://docs.chartbrew.com)