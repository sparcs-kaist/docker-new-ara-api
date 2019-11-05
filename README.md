# docker-new-ara-api

Automatic deployment of new-ara-api

## Notice

This repository does not `migrate`, `collectstatic`, or `createsuperuser` - you must do these outside containers created by this docker-compose. This is for auto-generated containers by auto-scaling, not for initial setup or development.

## Goal

* setup everything immediately after `docker-compose up`
