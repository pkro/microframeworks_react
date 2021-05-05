# Microfrontends with React: A Complete Developers Guide

## Overview

- Microfrontends split a monolithis single page application (SPA) up into independent ones with their own codebase
- each smaller app is responsible for a distict feature of the product
- communication happens over APIs (instead of a applicatoin state):

![communication of microfrontends](images/communication.png)

- Advantages
  - no need to stick to one framework
  - teams can work and deploy independently
  - less complexity, other parts aren't easily broken by making changes in another

- A container holds the microfrontends to decide when and where to show the microfrontends (*integration*)

![container](images/container.png)

- main categories solutions for integration:
  - build time integration:_**before** container gets loaded in the browser, it gets access to microfronteds source code)
  - run time integration (client side): **after** container gets loaded in the browser, it gets access to microfronteds source code)
  - Server integration: While sending down JS to load up container, server decides which MF to include


![build time integration](images/buildtimeintegration.png)

![build time integration](images/runtimeintegration.png)

## Course focus and project overview

Focus of the course is run-time integration using Webpack Module Federation

- hardest to set up and understand
- most flexible and performant
- needs good understanding of webpack

Example project structure:

![build time integration](images/projectoverview.png)

- no framework
- must be able to run in isolation
- must be able to be run in container app


