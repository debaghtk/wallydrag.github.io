---
layout: post
title: "Chef for the dumb minds"
description: ""
category: [Configuration management, devops, automation, Ruby]
tags: []
---
{% include JB/setup %}

Chef is a configuration management and automation tool that helps us to
manage complex infrastructure with the help of small snippets of codes
known as 'Recipies'. That makes our life easy (and tasty too).

Chef is primarily used by developers and organisations, to configure and
maintain their servers. It can integrate with multiple cloud-based
platforms, such as Amazon EC2, Rackspace to name a few. It has been
written in Ruby and Erlang and uses Ruby for writing recipies. Given the
large number of ruby developers and the compatibilty with other systems,
chef is really very popular. Whatever the size, chef automates how
applications are configured, deployed and managed across your network.

Recipies are snippets of codes written by user, that commands chef how a
server and its utilities are to be configured and managed. These
recipies when grouped together are called 'Cookbook'. (Try to get a hang
of the naming convention). A cookbook describes a series of resources
that should be in a particular state by ensuring the packages are
installed, services that should be running or files that should be
changed. Chef makes sure each resource is properly configured.

This next part that we will discuss is what sets apart chef from shell
cripting. ////////////////////////////////

Chef can run in client/server mode. A central chef server is located
attached to various instances of the user, called node. Each node has
chef client within. This chef client sends various attributes about the
state of the node, to the chef server. Chef provides an api to its user,
so that the user can query regarding the state of the node, and use the
data to configure the node.

ALso, if the user feels that he does not need so much functionality,
then also chef has a solution. Chef would then run in standalone
configuration called 'chef-solo'. This chef-solo is server-client
combined and useful for small scale. 
