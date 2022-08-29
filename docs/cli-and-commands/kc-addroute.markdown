---
layout: default
title: kc addroute
description: Description of the kc addroute command
parent: CLI and commands
last_modified_date: 2022-08-29 14:24
---

# kc addroute

## Feature

Create a new router for the nodejs project based on user answers

## Usage

{% highlight bash %}
$ kc addroute <router-name>
$ kc addr <router-name>
{% endhighlight %}

## Arguments

| Argument        | Description                                                                                               | Type     | Required |
| :-------------- | :-------------------------------------------------------------------------------------------------------- | :------- | -------- |
| `<router-name>` | path for the router to be created (ex : example/my-router). If not provided it will be asked to the user. | `string` | `false`  |

## Example

{% highlight bash %}
$ kc addr
{% endhighlight %}
