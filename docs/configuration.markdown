---
layout: default
title: Configuration
description: Configuration of the kestrel project.
last_modified_date: 2022-08-29 16:21
nav_order: 5
---

# Configuration of Kestrel
{: .no_toc }

Kestrel have many features built in. Here are the different configurations of those features.
{: .fs-6 .fw-300 }

---

## Table of contents
{: .no_toc  .text-delta}

- TOC
{:toc}

---

## Middlewares usage

### Global configuration

The global middlewares configuration is located at **backend/src/app.js** in the two const *back_config* and *middlewares*.

Activate or deactivate those configuration would affect the whole backend.

{% highlight js %}
// Don't change the order
const back_config = {
  helmet: true,
  swagger: true,
  session: true,
  cors: true,
  logger: true,
};

const middlewares = {
  checkToken: false,
  checkAuthenticated: false,
};
{% endhighlight %}

### Router configuration

The routers middlewares configuration is located at **backend/src/routes/routes.js**.

Activate or deactivate those configuration would affect all the routes of the router you modify.

{% highlight js %}
{
  checkToken: false,
  checkAuthenticated: false,
  path: 'example',
  router: 'example'
}
{% endhighlight %}

### Route configuration

You can specify routes's middlewares directly on the route function located at **backend/src/routes/\***.

{% highlight js %}
const checkAuthenticated = require('../configs/checkAuthenticated/checkAuthenticated');
router.get('/users', checkAuthenticated, async function (req, res, next) {
    ...
});
{% endhighlight %}

## Environment variables

You can edit the envronment variables in **backend/.env**.

{% highlight bash %}
# Env
NODE_ENV=dev
BLUEBIRD_W_FORGOTTEN_RETURN=0

# JWT
JWT_AUTHORIZATION_SERVER_URL=https://exemple.com
JWT_CLIENT_NAME=template_angular_node

# Mailer
SMTP_HOST=smtp.exemple.com
SMTP_PORT=25

# Api
API_VERSION=1.0
API_HOST=localhost
API_PORT=4000
API_BASE_PATH=/api
API_TITLE=Example Api for Template Angular Node
API_DESCRIPTION=Backend of the Template Angular Node
API_LOG_FILE=../access.log

# Session
SESSION_SECRET=c3cd31ea9300c9bc22c899ebbc570514b7d71090ccaafd6eb63c59dfa54251af

# BDD config DEVELOMENT
DB_USERNAME_DEV=
DB_PASSWORD_DEV=
DB_SCHEMA_DEV=
# https://sequelize.org/v5/manual/dialects.html
DB_DIALECT_DEV=mysql

# BDD config TEST
DB_USERNAME_TEST=
DB_PASSWORD_TEST=
DB_SCHEMA_TEST=
# https://sequelize.org/v5/manual/dialects.html
DB_DIALECT_TEST=mysql

# BDD config PRODUCTION
DB_USERNAME_PROD=
DB_PASSWORD_PROD=
DB_SCHEMA_PROD=
# https://sequelize.org/v5/manual/dialects.html
DB_DIALECT_PROD=mysql

# Crypto
SECRET_KEY=36355782fd6abadd871420fe9309e4fd
IV=084e9040dad528b3

# Encrypted data
EXAMPLE=ahu787d48a87ac8
{% endhighlight %}
