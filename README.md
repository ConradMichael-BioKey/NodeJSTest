# Technical Test: Node.js/API Development and DevOps

## Overview

This technical test is designed to evaluate your skills in Node.js/API development with an additional focus on DevOps practices, particularly containerization using Docker. You will be required to create a simple REST API and then dockerize your application.

## Submission Instructions

- **Repository:** Provide a GitHub repository link with the complete project code, Dockerfiles, docker-compose file, and any additional documentation.
- **README.md:** Ensure it clearly explains how to set up and run your application, including any prerequisites and how to execute your deployment script.

## Part 1: Node.js and API Development

### Objective

Create a REST API to manage a basic resource (e.g., users, tasks, products) with CRUD (Create, Read, Update, Delete) functionality.

### Requirements

#### API Specification

- **Framework:** Use Express.js (or Fastify if preferred).
- **Endpoints:** Define routes for creating, retrieving, updating, and deleting items of the chosen resource.
- **Validation:** Use a validation library (e.g., Joi, Zod, express-validator) to validate incoming request data.

#### Data Storage

- **Database:** Use SQLite for data storage (via Sequelize, Prisma, or better-sqlite3).
- **Schema:** Design a simple schema relevant to the managed resource.

#### Testing

- **Framework:** Write unit and integration tests using Jest, Mocha, or a similar Node.js testing framework.
- **Coverage:** Ensure tests cover all core API functionalities.

## Part 2: DevOps Integration

### Objective

Containerize the API application using Docker to ensure easy setup and environment consistency.

### Requirements

#### Dockerfile

- Create a Dockerfile for your Node.js application, optimizing for minimal image size (e.g., use `node:alpine`).

#### Docker Compose

- **Compose File:** Create a `docker-compose.yml` file to run the API and mount a persistent volume for SQLite.
- **Volumes:** Use volumes to persist database data and optionally enable live code reloading (e.g., using `nodemon` in dev).

#### Deployment Script

- **Script:** Write a script (bash or shell) to build the Docker image, run the containers, and make a test request to confirm the API is operational.

#### Bonus: CI/CD Integration (Optional)

- Set up a basic CI/CD pipeline (e.g., GitHub Actions, GitLab CI/CD) to build the Docker image and run tests on push or pull requests.

## Evaluation Criteria

- **Code Quality:** Clean, maintainable, and idiomatic Node.js code.
- **Functionality:** Correct CRUD operations and API behavior.
- **Error Handling:** Meaningful and consistent error handling.
- **Docker Integration:** Well-structured Dockerfile and docker-compose setup.
- **Documentation:** Clear instructions in the README for setup, running, and testing.
