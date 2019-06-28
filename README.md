# Mongo Chart
MongoDB Helm chart.

# Table Of Contents
- [Overview](#overview)
- [Use](#use)

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
