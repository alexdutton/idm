[![Stories in Ready](https://badge.waffle.io/alexsdutton/idm.png?label=ready&title=Ready)](https://waffle.io/alexsdutton/idm?utm_source=badge)
# IdM

This is a collection of web applications and APIs that together form a proof of
concept for an Identity Management System. It aims towards implementing and
supporting the [IAM Process, Policy and
Governance](https://ox-it.github.io/iam-ppg) documents.

It comprises:

Project | Badges | Description
--- | --- | ---
[idm-core](https://github.com/alexsdutton/idm-core) | [![Build Status](https://travis-ci.org/alexsdutton/idm-core.svg?branch=master)](https://travis-ci.org/alexsdutton/idm-core) [![codecov](https://codecov.io/gh/alexsdutton/idm-core/branch/master/graph/badge.svg)](https://codecov.io/gh/alexsdutton/idm-core) | The core Identity store, exposed through a self-service and devolved administrator web interface, and a `django-rest-framework`-based API.
[idm-auth](https://github.com/alexsdutton/idm-auth) | [![Build Status](https://travis-ci.org/alexsdutton/idm-auth.svg?branch=master)](https://travis-ci.org/alexsdutton/idm-auth) [![codecov](https://codecov.io/gh/alexsdutton/idm-auth/branch/master/graph/badge.svg)](https://codecov.io/gh/alexsdutton/idm-auth) [![Codacy Badge](https://api.codacy.com/project/badge/Grade/862642b5c38140cfa5549048c07f361b)](https://www.codacy.com/app/alexsdutton/idm-auth) | An authentication component, which provides onboarding, self-registration, authentication and OpenID Connect OP functionality on top of idm-core.
[idm-card](https://github.com/alexsdutton/idm-card) | [![Build Status](https://travis-ci.org/alexsdutton/idm-card.svg?branch=master)](https://travis-ci.org/alexsdutton/idm-card) [![codecov](https://codecov.io/gh/alexsdutton/idm-card/branch/master/graph/badge.svg)](https://codecov.io/gh/alexsdutton/idm-card) | A University and Bodleian Card management application (early days)
[idm-broker](https://github.com/alexsdutton/idm-broker) | [![Build Status](https://travis-ci.org/alexsdutton/idm-broker.svg?branch=master)](https://travis-ci.org/alexsdutton/idm-broker) [![codecov](https://codecov.io/gh/alexsdutton/idm-broker/branch/master/graph/badge.svg)](https://codecov.io/gh/alexsdutton/idm-broker) [![Codacy Badge](https://api.codacy.com/project/badge/Grade/beaa12a3f44e4296abe601bed0f9d309)](https://www.codacy.com/app/alexsdutton/idm-broker) [![Documentation Status](https://readthedocs.org/projects/alexsdutton-idm-broker/badge/?version=latest)](http://alexsdutton-idm-broker.readthedocs.io/en/latest/?badge=latest) | A supporting reusable Django application for publishing model changes to an AMQP message broker, and consuming AMQP queues to turn into Celery tasks.
[idm-brand](https://github.com/alexsdutton/idm-brand) | [![Build Status](https://travis-ci.org/alexsdutton/idm-brand.svg?branch=master)](https://travis-ci.org/alexsdutton/idm-brand) [![codecov](https://codecov.io/gh/alexsdutton/idm-brand/branch/master/graph/badge.svg)](https://codecov.io/gh/alexsdutton/idm-brand) | Common templates and static files, providing a branded basis for the user interfaces.
[idm-integration](https://github.com/alexsdutton/idm-integration) | [![Build Status](https://travis-ci.org/alexsdutton/idm-integration.svg?branch=master)](https://travis-ci.org/alexsdutton/idm-integration) [![codecov](https://codecov.io/gh/alexsdutton/idm-integration/branch/master/graph/badge.svg)](https://codecov.io/gh/alexsdutton/idm-integration) | Tasks for integrating with other (concrete) systems. Currently only importing the University of Oxford's organisation chart is possible.
[django-camera-imagefield](https://github.com/alexsdutton/django-camera-imagefield) | [![Build Status](https://travis-ci.org/alexsdutton/django-camera-imagefield.svg?branch=master)](https://travis-ci.org/alexsdutton/django-camera-imagefield) [![codecov](https://codecov.io/gh/alexsdutton/django-camera-imagefield/branch/master/graph/badge.svg)](https://codecov.io/gh/alexsdutton/django-camera-imagefield) [![Codacy Badge](https://api.codacy.com/project/badge/Grade/55d2b6a967a94baa99a0bbb280527aef)](https://www.codacy.com/app/alexsdutton/django-camera-imagefield) [![PyPI](https://img.shields.io/pypi/v/django-camera-imagefield.svg)](https://pypi.python.org/pypi/django-camera-imagefield) | Django field and widget that can capture images from a device's camera

Integration between components is done using HTTP RESTful APIs for
client-server changes and AMQP for real-time publish/subscribe.

Everything is written (so far) using Python and Django, reusing existing
components wherever possible. Each idm-\* component should be minimal and
concise.

## Test coverage sunbursts

[![codecov for idm-core](https://codecov.io/gh/alexsdutton/idm-core/branch/master/graphs/sunburst.svg)](https://codecov.io/gh/alexsdutton/idm-core)
[![codecov for idm-auth](https://codecov.io/gh/alexsdutton/idm-auth/branch/master/graphs/sunburst.svg)](https://codecov.io/gh/alexsdutton/idm-auth)
[![codecov for idm-card](https://codecov.io/gh/alexsdutton/idm-card/branch/master/graphs/sunburst.svg)](https://codecov.io/gh/alexsdutton/idm-card)
[![codecov for idm-broker](https://codecov.io/gh/alexsdutton/idm-broker/branch/master/graphs/sunburst.svg)](https://codecov.io/gh/alexsdutton/idm-broker)
