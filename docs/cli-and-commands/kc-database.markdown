---
layout: default
title: kc database
description: Description of the kc database command
parent: CLI and commands
last_modified_date: 2022-08-29 14:18
---

# kc database

## Feature

Run [commands](https://www.npmjs.com/package/sequelize-cli#usage) with the sequelize-cli and sequelize-auto

## Usage

{% highlight bash %}
$ kc database [options] <command> [sequelize-options]
$ kc db [options] <command> [sequelize-options]
{% endhighlight %}

## Arguments

| Argument    | Description                                                                                                       | Type     | Required |
| :---------- | :---------------------------------------------------------------------------------------------------------------- | :------- | -------- |
| `<command>` | sequelize command to run with its options ([see ORM commands](https://www.npmjs.com/package/sequelize-cli#usage)) | `string` | `true`   |

## Options

| Option        | Description                                                                |
| :------------ | :------------------------------------------------------------------------- |
| `--env <env>` | env to use when interacting the database (dev, test, prod). Default is dev |

## Example

{% highlight bash %}
$ kc database --env dev migration:generate --name create-users
{% endhighlight %}
