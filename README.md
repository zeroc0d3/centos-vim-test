# CentOS Vim Docker (Vim Container)
[![Build Status](https://travis-ci.org/zeroc0d3/centos-vim-test.svg?branch=master)](https://travis-ci.org/zeroc0d3/centos-vim-test) [![](https://images.microbadger.com/badges/image/zeroc0d3/centos-vim-test:latest.svg)](https://microbadger.com/images/zeroc0d3/centos-vim-test:latest "Layers") [![](https://images.microbadger.com/badges/version/zeroc0d3/centos-vim-test:latest.svg)](https://microbadger.com/images/zeroc0d3/centos-vim-test:latest "Version") [![GitHub issues](https://img.shields.io/github/issues/zeroc0d3/centos-vim-test.svg)](https://github.com/zeroc0d3/centos-vim-test/issues) [![GitHub forks](https://img.shields.io/github/forks/zeroc0d3/centos-vim-test.svg)](https://github.com/zeroc0d3/centos-vim-test/network) [![GitHub stars](https://img.shields.io/github/stars/zeroc0d3/centos-vim-test.svg)](https://github.com/zeroc0d3/centos-vim-test/stargazers) [![GitHub license](https://img.shields.io/badge/license-GPLv2-blue.svg)](https://raw.githubusercontent.com/zeroc0d3/centos-vim-test/master/LICENSE)

This docker image includes:

## Features:
* bash (+ themes)
* oh-my-zsh (+ themes)
* tmux (+ themes)
* vim (+ plugins with vundle & themes)

## Docker Compose
* Copy `env-example` to `.env`
* Build & running
  ```
  docker-compose build && docker-compose up
  ```
* Force recreate container
  ```
  docker-compose build && docker-compose up --force-recreate vim
  ```
* Running container only
  ```
  docker-compose up
  ```

## Environments
You can run docker-compose for different environment with selected containers
* Copy `env.sh.example` to `env.sh`
* Change to execute script
  ```
  chmod a+x env.sh
  ```
* Change environment in `env.sh` file
  ```
  ENV="development"            # (use: "development" or "production" as selected environment)
  CONTAINER_PRODUCTION="..."   # (selected containers will be run in production environment)
  CONTAINER_DEVELOPMENT="..."  # (selected containers will be run in development environment)
  ```
* Running script
  ```
  ./env.sh
  ```

## License
[**GNU General Public License v2**](https://github.com/zeroc0d3/centos-vim-test/blob/master/LICENSE)