---
layout: post
title: Starting with Jenkins pipelines
date: '2016-11-03 19:24:39 +0200'
author: jovandeginste
comments: true
tags:
  - jenkins
published: true
---

Getting started with Jenkins pipelines was daunting at first. A new language (Groovy) for me, and a new job type. Online support was hard to find or simply lacking. However, some things help you a long way!

## Replay

When a Jenkins job is converted to a pipeline job, you will have among the extra options is one that will help you out a lot: "replay". You find it when focusing a specific build.

Clicking the "replay" option will show you all relevant Pipeline files, each in an editable text area. This means you can edit them live (without committing them your repository) and then run a build using the edited versions.

You can iterate further by replaying the edited run, or view the differences in order to persist them in your code repository.

This feature allows for fast debugging and iteration without mudding your code repository. Very useful when learning the language, DSL and workflows.

## Pipeline syntax

This is another feature in Jenkins, where you get a kind of wizard that generates Groovy snippets. You can access it when focusing a job (not a build) or from the replay page.

It is self explaining: you select a function from the core or from a plugin, fill in the parameters in the input fields and click "Generate Pipeline Script". Guess what it does: it generates a code snippet ready to copy and paste.

It gives you quick access to the DSL so you don't have to dive into the source code or find other people's examples.