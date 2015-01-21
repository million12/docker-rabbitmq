# RabbitMQ on CentOS-7 | Docker image
[![Circle CI](https://circleci.com/gh/million12/docker-rabbitmq.svg?style=svg)](https://circleci.com/gh/million12/docker-rabbitmq)

RabbitMQ built on CentOS-7, with an **ability to execute arbitrary commands just after RabbitMQ has started**.

## Features

* Default user `guest` removed
* User `admin:password` added. Modify the password by setting `RABBITMQ_PASS`
* Extra args passed to `docker run` or via `USER_COMMANDS` will be executed just after RabbitMQ has started.  
  That gives you handy opportunity to pre-configure RabbitMQ to your needs, e.g. by calling `rabbitmqctl add_vhost` etc.  
  See [circle.yml](circle.yml) for examples.

## Authors

Author: Marcin Ryzycki (<marcin@m12.io>)  
Author: Przemyslaw Ozgo (<linux@ozgo.info>)

---

**Sponsored by** [Typostrap.io - the new prototyping tool](http://typostrap.io/) for building highly-interactive prototypes of your website or web app. Built on top of TYPO3 Neos CMS and Zurb Foundation framework.
