# event-manager <img src="https://github.com/alice-biometrics/custom-emojis/blob/master/images/rabbitmq.png" width="26">  [![ci](https://github.com/alice-biometrics/petisco-task-manager/workflows/ci/badge.svg)](https://github.com/alice-biometrics/petisco-task-manager/actions)

<img src="https://github.com/alice-biometrics/custom-emojis/blob/master/images/alice_header.png" width=auto>

ALiCE Event Manager.

## Table of Contents
- [Application :rocket:](#application-rocket)
- [Installation :computer:](#installation-computer)
- [Testing :white_check_mark:](#testing-white_check_mark)
- [Configuration :gear:](#configuration-gear)
- [Contact :mailbox_with_mail:](#contact-mailbox_with_mail)


## Application :rocket:

This service do no expose any entry point. It works reading events from rabbitmq queues.

Subscriptors:
* TODO


## Installation :computer:

Use [lume :fire:](https://github.com/alice-biometrics/lume) to install dependencies:

Example:

```console
>> conda create -n myenv python=3.6
>> conda activate myenv
(myenv) >> lume -install # pip install lume if needed
```

## Testing :white_check_mark:

### Unit, Integration and Acceptance

```console
(myenv) >> lume -test
```

### End-to-end [python]

```console
(myenv) >> lume -test-e2e-local-python
```

### End-to-end [docker-compose]

```console
(myenv) >> lume -test-e2e-local
```

## Configuration :gear:

Application can be configured by *environment variables*.

* Petisco :cookie:
  * `PETISCO_PORT: "8080"`
* Event Manager <img src="https://github.com/alice-biometrics/custom-emojis/blob/master/images/rabbitmq.png" width="16">
:
  * `EVENT_MANAGER_TYPE: "rabbitmq"` (By default it uses a not implemented event manager)
  * `RABBITMQ_USER: "guest"`
  * `RABBITMQ_HOST: "localhost"`
  * `RABBITMQ_PORT: "5672"`
  * `RABBITMQ_DEPLOY_TOPIC: "deploy"`

## Contact :mailbox_with_mail:

support@alicebiometrics.com

