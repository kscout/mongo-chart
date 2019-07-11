# Mongo Chart
MongoDB Helm chart.

# Table Of Contents
- [Overview](#overview)
- [Use](#use)
- [Release Checklist](#release-checklist)

# Overview
Many of our services require their own Mongo DB instance be deployed.  

This repository contains a Helm chart which deploys MongoDB.

# Use
Complete the following steps to use the Mongo chart:

1. Add this repository as a Git submodule:
   ```
   git submodule add git@github.com:kscout/mongo-chart.git <your chart path>/charts/mongo
   ```
   Be sure to replace `<your chart path>` with the path to your
   repository's chart.
2. Set the `global.env` and `global.app` values
3. Set the `mongo.dbPassword` value

# Release Checklist
When a new release occurs:

1. Bump `version` in [`Chart.yaml`](Chart.yaml)
2. [Create release](https://github.com/kscout/http-service-chart/releases/new) 
   tagged `v<chart version>`
3. Update submodules and open PR for the following repositories:
   - [chat-bot-api](https://github.com/kscout/chat-bot-api)
   - [serverless-registry-api](https://github.com/kscout/serverless-registry-api)
