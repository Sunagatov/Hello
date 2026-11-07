# Hello — CI/CD Sample Application

A minimal Spring Boot service used to demonstrate a Java build and deployment pipeline.

<p>
  <a href="https://buymeacoffee.com/lucky_1uck">
    <img src="https://img.shields.io/badge/Support_the_project-FFDD00?style=for-the-badge&amp;logo=buymeacoffee&amp;logoColor=black" alt="Support the project" width="260" height="40">
  </a>
</p>

## What it does

`GET /` returns:

```text
Hello World!
```

The project includes Spring Boot Actuator, the Micrometer Prometheus registry
and a Dockerfile so the service can be used in deployment and monitoring exercises.

## Run locally

Install JDK 11 and Maven:

```bash
mvn package
mvn spring-boot:run
```

Open `http://localhost:8080/`, or check the endpoint from a terminal:

```bash
curl http://localhost:8080/
```

## Build a container

After the Maven build:

```bash
docker build -t hello .
docker run --rm -p 8080:8080 hello
```

## Read the walkthrough

The accompanying article explains the larger pipeline with AWS, Kubernetes,
Docker, Ansible, Git, Maven and Jenkins:

[Building a CI/CD Pipeline](https://hackernoon.com/building-a-cicd-pipeline-with-aws-k8s-docker-ansible-git-github-apache-maven-and-jenkins).

For supporting setup guides, see [DevOps](https://github.com/Sunagatov/DevOps).
This repository contains the sample application; the full pipeline is described
in those resources.

## ☕ Support the project

If this project helps you learn or build, you can support its development.

<p>
  <a href="https://buymeacoffee.com/lucky_1uck">
    <img src="https://img.shields.io/badge/Support_the_project-FFDD00?style=for-the-badge&amp;logo=buymeacoffee&amp;logoColor=black" alt="Support the project" width="260" height="40">
  </a>
</p>
