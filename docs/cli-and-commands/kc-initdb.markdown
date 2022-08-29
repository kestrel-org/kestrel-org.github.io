---
layout: default
title: kc initdb
description: Description of the kc innitdb command
parent: CLI and commands
last_modified_date: 2022-08-29 13:54
---

# kc initdb

## Feature

Create or replace the database with the sequelize's migrations and seeders

## Usage

{% highlight bash %}
$ kc initdb [options]
$ kc idb [options]
{% endhighlight %}

## Options

| Option                | Description                                                                 |
| :-------------------- | :-------------------------------------------------------------------------- |
| `--env <env>`         | env to use when initialising the database (dev, test, prod). Default is dev |
| `--ignore-list` `--il` | ignore all or several seeders during init                                   |

## Example

{% highlight bash %}
$ kc initdb --env prod
{% endhighlight %}
