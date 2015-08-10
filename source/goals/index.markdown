---
layout: page
title: "goals"
date: 2015-08-10 12:15
comments: true
sharing: true
footer: true
---

This is a high-level, rough and time-boxed list of goals. Any part of it can
change at any point of time as a response to change.

## From zero to deployed "Hello world" web-nanoservice in 5 minutes

I want to be able to setup my cluster in 5 minutes and it should have a default
"Hello world" web-nanoservice and I want to be able to jump in and play around
with it right away.

Milestone: 31.08.15.

## From zero to deployed application prototype consisting of ~10 nanoservices communicating over the bus in 4 hours

I want to be able to bootstrap new nanoservice with one command. I want to be
able to jump in and modify nanoservice to do its job and deploy it in ~30
minutes.

Milestone: 21.09.15.

## Low latency (~5-20 ms per enhancement hop) communication between nanoservices

I want to be able to build parallel message enhancement chains of up to 4
times. To maintain fast response time of the whole system, I need to have low
latency for message passing.

Milestone: 28.09.15.

## Monitoring of all nanoservices and supporting systems without any additional setup

I want to be able to see health of all nanoservices I create without any setup
required from me. Also I want to be able to see health of all supporting
systems that power my cluster.

Milestone: 05.10.15.

## Dashboard with all application KPIs in 30 minutes

I want to be able to configure dashboard, that will contain all the KPIs
represented with graphs. These should be based on events emitted by my
nanoservices.

Milestone: 26.10.15.

## Effortless autoscaling

I want to be able to enable and configure autoscaling for my nanoservices.
Configuring means setting up maximum allowed amount of instances. It should
scale accordingly to increased load on concrete nanoservice up and down. At
this point, 2 instances is a minimum scaling factor for each nanoservice,
unless specifically opted out.

Milestone: 09.11.15.

## Self-healing cluster

I want my nanoservice instances to automatically be launched when dead. I don't
want to be required to take any action for that.

Milestone: 16.11.15.

## Canari deployments

I want to be able to deploy a new version of a given nanoservice without
affecting majority of my traffic. Slowly over time, new version should take
over the traffic unless cancelled by me. I want to be able to see new version's
health and KPIs compared to current one.

Milestone: 07.12.15

## Hosted solution + easy to catch & use documentations

I want to be able to deploy my cluster without actually buying hardware or
signing up for cloud provider myself. I want just pay small additional cost for
operations and deploy to hosted cluster.

Milestone: 01.04.16.

## TODO

 * Specify objectives for couple of first goals in separate pages and link them
from here.
