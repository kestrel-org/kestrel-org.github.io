---
layout: default
title: kc new
description: Description of the kc new command
parent: CLI and commands
last_modified_date: 2022-08-29 13:44
---

# kc new

## Feature

Create new project based on the angular/nodejs template

## Usage

{% highlight bash %}
$ kc new <project-name> [options]
$ kc n <project-name> [options]
{% endhighlight %}

## Arguments

| Argument         | Description             | Type     | Required |
| :--------------- | :---------------------- | :------- | -------- |
| `<project-name>` | name of the new project | `string` | `true`   |

## Options

| Option         | Description                    |
| :------------- | :----------------------------- |
| `--back` `-b`  | generate only the nodejs part  |
| `--front` `-f` | generate only the angular part |

## Example

{% highlight bash %}
$ kc new my-awesome-project
{% endhighlight %}
