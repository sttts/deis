# Test Plan for Deis

Version: 0.1

2014-05-23

## Introduction

Deis (pronounced DAY-iss) is an open source PaaS that makes it easy to deploy
and manage applications on your own servers. Deis builds upon
[Docker](http://docker.io/) and [CoreOS](http://coreos.com) to provide a
lightweight PaaS with a [Heroku-inspired](http://heroku.com) workflow.

This document is a test plan for the Deis system, with a particular focus on
test automation.

### Objectives
This test plan describes all software testing activities planned for the near
future of the Deis project. The complete implementation of this test plan should
ensure rapid feedback on the quality of proposed changes and enable releases of
Deis to meet well-defined quality standards.

### Background
Early on, testing of Deis was mostly manual. Unit tests for the main controller
component were created using Django's test framework. These tests, combined with
test coverage, were automated and continue to run at
[Travis CI](http://travis-ci.org/). But maintainers executed an acceptance
checklist by hand at release time and did ad-hoc testing for proposed
 code changes.

Deis has become popular rapidly thanks to Deis' core team of maintainers:
capable developers who consistently deliver features and fixes in a short time.
But test infrastructure has not kept up with the growth of Deis, and these gaps
in automation mean that maintainers may spend most of their time manually
testing each others' changes to verify quality.

### Scope
A test of the Deis system has the objective to show that when the software is
deployed to a cluster of machines it behaves as a Heroku-like PaaS
(Platform-as-a-Service) that enables a variety of applications to be deployed,
configured, revised, and scaled.

As an agile open source project, Deis has no overall product specification
document. So a secondary goal of the test plan is to codify those behaviors that
are essential to the Deis system.

### References
- [Deis website](http://deis.io/)
- [Deis project](http://github.com/deis/deis/)
- [Deis documentation](http://docs.deis.io/)
- [Heroku](https://www.heroku.com/)
- [PaaS](https://en.wikipedia.org/wiki/Platform_as_a_service)


## Test Items

The software item to be used for testing is a particular code revision of the
Deis project, specifically a git SHA referencing the
[master repository](https://github.com/deis/deis).


## Features To Be Tested

- one
- two
- three


## Features Not To Be Tested

## Approach / Testing Strategy


## Item Pass / Fail Criteria

## Suspension Criteria & Resumption Requirements

## Test Deliverables

## Testing Tasks

## Environmental Needs

## Responsibilities

## Staffing & Training Needs

## Schedule

## Risks & Contingencies

## Approvals
