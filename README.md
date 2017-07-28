# IdM

This is a collection of web applications and APIs that together form a proof of
concept for an Identity Management System. It aims towards implementing and
supporting the [IAM Process, Policy and
Governance](https://ox-it.github.io/iam-ppg) documents.

It comprises:

Project | Badges | Description
--- | --- | ---
[idm-core](https://github.com/alexsdutton/idm-core) | [![Build Status](https://travis-ci.org/alexsdutton/idm-core.svg?branch=master)](https://travis-ci.org/alexsdutton/idm-core) [![codecov](https://codecov.io/gh/alexsdutton/idm-core/branch/master/graph/badge.svg)](https://codecov.io/gh/alexsdutton/idm-core) | The core Identity store, exposed through an API.
[idm-auth](https://github.com/alexsdutton/idm-auth) | [![Build Status](https://travis-ci.org/alexsdutton/idm-auth.svg?branch=master)](https://travis-ci.org/alexsdutton/idm-auth) [![codecov](https://codecov.io/gh/alexsdutton/idm-auth/branch/master/graph/badge.svg)](https://codecov.io/gh/alexsdutton/idm-auth) | An authentication component, which provides onboarding, self-registration, authentication and IdP functionality on top of idm-core.
[idm-card](https://github.com/alexsdutton/idm-card) | [![Build Status](https://travis-ci.org/alexsdutton/idm-card.svg?branch=master)](https://travis-ci.org/alexsdutton/idm-card) [![codecov](https://codecov.io/gh/alexsdutton/idm-card/branch/master/graph/badge.svg)](https://codecov.io/gh/alexsdutton/idm-card) | A University and Bodleian Card management application (early days)
[idm-broker](https://github.com/alexsdutton/idm-broker) | [![Build Status](https://travis-ci.org/alexsdutton/idm-broker.svg?branch=master)](https://travis-ci.org/alexsdutton/idm-broker) [![codecov](https://codecov.io/gh/alexsdutton/idm-broker/branch/master/graph/badge.svg)](https://codecov.io/gh/alexsdutton/idm-broker) | A supporting Django application for publishing model changes to an AMQP message broker.
[idm-brand](https://github.com/alexsdutton/idm-brand) | [![Build Status](https://travis-ci.org/alexsdutton/idm-brand.svg?branch=master)](https://travis-ci.org/alexsdutton/idm-brand) [![codecov](https://codecov.io/gh/alexsdutton/idm-brand/branch/master/graph/badge.svg)](https://codecov.io/gh/alexsdutton/idm-brand) | Common templates and static files, providing a branded basis for the user interfaces.

Integration between components is done using HTTP RESTful APIs for
client-server changes and AMQP for real-time publish/subscribe.

Everything is written (so far) using Python and Django, reusing existing
components wherever possible. Each idm-\* component should be minimal and
concise.

