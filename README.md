# egeoffrey-interaction-telegram

This is an eGeoffrey interaction package.

## Description

Connect to a Telegram group as a bot and interact with the users.

## Install

To install this package, run the following command from within your eGeoffrey installation directory:
```
egeoffrey-cli install egeoffrey-interaction-telegram
```
After the installation, remember to run also `egeoffrey-cli start` to ensure the Docker image of the package is effectively downloaded and started.
To validate the installation, go and visit the *'eGeoffrey Admin'* / *'Packages'* page of your eGeoffrey instance. All the modules, default configuration files and out-of-the-box contents if any will be automatically deployed and made available.
## Content

The following modules are included in this package.

For each module, if requiring a configuration file to start, its settings will be listed under *'Module configuration'*. Additionally, if the module is a service, the configuration expected to be provided by each registered sensor associated to the service is listed under *'Service configuration'*.

To configure each module included in this package, once started, click on the *'Edit Configuration'* button on the *'eGeoffrey Admin'* / *'Modules'* page of your eGeoffrey instance.
- **interaction/telegram_messenger**: connect to a Telegram group as a bot and interact with the user
  - Module configuration:
    - *bot_token**: the token of the Telegram bot you have created (https://core.telegram.org/bots#3-how-do-i-create-a-bot)
    - *command_handler**: the command to use as a prefix for interacting with the bot (e.g. /housebot hi) (e.g. housebot)

## Contribute

If you are the author of this package, simply clone the repository, apply any change you would need and run the following command from within this package's directory to commit your changes and automatically push them to Github:
```
egeoffrey-cli commit "<comment>"
```
After taking this action, remember you still need to build (see below) the package (e.g. the Docker image) to make it available for installation.

If you are a user willing to contribute to somebody's else package, submit your PR (Pull Request); the author will take care of validating your contributation, merging the new content and building a new version.

## Build

Building is required only if you are the author of the package. To build a Docker image and automatically push it to [Docker Hub](https://hub.docker.com/r/egeoffrey/egeoffrey-interaction-telegram), run the following command from within this package's directory:
```
egeoffrey-cli build egeoffrey-interaction-telegram
```

## Uninstall

To uninstall this package, run the following command from within your eGeoffrey installation directory:
```
egeoffrey-cli uninstall egeoffrey-interaction-telegram
```
Remember to run also `egeoffrey-cli start` to ensure the changes are correctly applied.
## Tags

The following tags are associated to this package:
```
interaction telegram
```

## Version

The version of this egeoffrey-interaction-telegram is 1.1-2 on the master branch.
