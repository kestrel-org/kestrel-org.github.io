---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Getting started
description: Quick install guide for testing the kestrel project. Test it now !
last_modified_date: 2022-08-29 10:20
nav_order: 2
---

# Getting started

## Prerequisities

- Latest LTS of [Node.js](https://nodejs.org/en/)
- [Nodemon](https://www.npmjs.com/package/nodemon) globally installed
- Any kind of SGDB installed

## Step 1 - Install the kestrel-cli

Run the following command to install our cli.

{% highlight bash %}
npm install --location=global @kestrels/cli
{% endhighlight %}

## Step 2 - Create a new project

Run the following command to create a new project with our cli.

{% highlight bash %}
kc new <project_name>
{% endhighlight %}

## Step 3 - Configure the database access

You can configure the database access in **backend/.env**.

{% highlight env %}

# BDD config DEVELOMENT

DB_USERNAME_DEV=
DB_PASSWORD_DEV=
DB_SCHEMA_DEV=

# https://sequelize.org/v5/manual/dialects.html

DB_DIALECT_DEV=mysql
{% endhighlight %}

## Step 4 - Initialize the database

You can run the following command to initialize the databse with our cli.

{% highlight bash %}
kc initdb
{% endhighlight %}

## Step 5 - Running the app

After the setup done, you can start app by running the following command.

{% highlight bash %}
kc start
{% endhighlight %}

By default you can access the backend on [http://localhost:4000](http://localhost:4000) and the frontend on [http://localhost:4200](http://localhost:4200).

The API documentation can be accessed on [http://localhost:4000/api-docs](http://localhost:4000/api-docs).
