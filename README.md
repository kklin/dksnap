# ![dksnap logo](https://kelda.io/img/dksnap/dksnap-logo.svg)
[![Build Status](https://travis-ci.org/kelda/dksnap.svg?branch=master)](https://travis-ci.org/kelda/dksnap)
[![Go Report Card](https://goreportcard.com/badge/github.com/kelda/dksnap)](https://goreportcard.com/report/github.com/kelda/dksnap)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![Slack](https://kelda.io/img/dksnap/slack-badge.svg)](http://slack.kelda.io)
[![Made by Kelda](https://kelda.io/img/dksnap/love-badge.svg)](https://kelda.io)

[![Demo Gif](https://kelda.io/img/dksnap/create-snapshot.gif)](https://youtu.be/EaxEsOTKdrs)

### Docker Snapshots for Test Databases

`dksnap` allows you to create, view, and run snapshots of docker containers.

- TODO Outline
    - Typically when developing, particulary with docker compose, you've got a
      database container that you're testing against.
    - It's often really difficult and slow to setup, and generally painful to
      manipulate
    - dk Snapshot let's you take a snapshot of a database you're working on at
      a useful state, and then roll back or roll forward as needed.

For a full description of why we built this, check out our [blogpost](TODO)

DKsnap is in alpha, but ready for the most adventerous users.  Please report
bugs!

## Install
Install on MacOS or Linux:

```
curl https://kelda.io/install-dksnap.sh | sh
```

Or download the latest [release](https://github.com/kelda/dksnap/releases) and
copy to your path.

### Demo
Recreate the [demo](https://youtu.be/EaxEsOTKdrs) locally.

```
git clone https://github.com/kelda/dksnap.git
cd dksnap/demo
docker-compose up -d
dksnap
```

## Features

### Create Snapshot
![](https://kelda.io/img/dksnap/create-snapshot.gif)
TODO short description

### View History
TODO short description
![](https://kelda.io/img/dksnap/view-history.gif)

### Boot Snapshot
![](https://kelda.io/img/dksnap/boot-snapshot.gif)
TODO short description

### Swap Snapshot
![](https://kelda.io/img/dksnap/swap-snapshot.gif)
TODO short description

### Share Snapshots
![](https://kelda.io/img/dksnap/share-snapshot.gif)

### Database Aawareness
TODO mention that dksnap is DB aware for the following

It also has a fallback mode that works for every container, 
some featuers don't work in that case.

## FAQ

- How is this different then?
    - docker commit?

- Can I use this with?


- TODO what else?


## Contributing

### Build

`dksnap` uses Go Modules which were introduced in `go` version 1.11.

```
git clone https://github.com/kelda/dksnap
cd dksnap
GO111MODULE=on go install .
dksnap
```

### TODO What else should we say in Contributing?

## Roadmap

# TODOs
- Badges
- Licencse
- "Test DB Management with Docker Snapshots" isn't working for me.
- test all of the install scripts.
- Host mages on kelda.io instead of in git repo.  Squash commits to achieve this.
- TODO shrink example gifs

TODO deal with below
