# Invoicer Auth

[![Build Status](https://travis-ci.org/caelwinner/invoicer-auth.svg?branch=master)](https://travis-ci.org/caelwinner/invoicer-auth)

## Overview

OAuth2 server powered by Spring Boot 2 and using base-auth2-server library

## Requierments
- Docker 1.7
- Java 1.8


## Build and Run docker image

In order to build and image use:
- ./gradlew buildDocker

if you want to push it
- docker push adolfoecs/invoicer-auth:0.1.0-SNAPSHOT

In order to run the image use:

- docker run -p 8580 --name invoicer-auth-instance1 -t adolfoecs/invoicer-auth:0.1.0-SNAPSHOT

## Running

In order to run the app just execute:

./gradlew bootrun

To build a jar and run all the tests (Unit and e2e):

./gradlew test assemble

the application run on http://localhost:8080.