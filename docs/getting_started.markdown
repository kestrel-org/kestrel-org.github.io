---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Getting started
description: Quick install guide for testing the kestrel project. Test it now !
last_modified_date: 2022-08-29 12:10
nav_order: 2
---

# Getting started

This page aims to give a quick install guide for testing the kestrel project.
{: .fs-6 .fw-300 }

---

## Prerequisities

- Latest LTS of [Node.js](https://nodejs.org/en/)
- [Nodemon](https://www.npmjs.com/package/nodemon) globally installed
- Any kind of database installed

---

1- Install the kestrel-cli
{% highlight bash %}
$ npm install -g @kestrels/cli
{% endhighlight %}

2- Create a new project
{% highlight bash %}
$ kc new <project_name>
{% endhighlight %}

3- Configure the database access in **backend/.env**
{% highlight env %}

# BDD config DEVELOMENT
DB_USERNAME_DEV=
DB_PASSWORD_DEV=
DB_SCHEMA_DEV=

# https://sequelize.org/v5/manual/dialects.html
DB_DIALECT_DEV=mysql
{% endhighlight %}

4- Initialize the database
{% highlight bash %}
$ kc initdb
{% endhighlight %}

5- Running the app
{% highlight bash %}
$ kc start
{% endhighlight %}

6- Point your web browser to [http://localhost:4200](http://localhost:4200).

By default you can access the _backend_ on [http://localhost:4000](http://localhost:4000) and the _frontend_ on [http://localhost:4200](http://localhost:4200).

The _API documentation_ can be accessed on [http://localhost:4000/api-docs](http://localhost:4000/api-docs).
