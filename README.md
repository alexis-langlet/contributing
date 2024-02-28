# Contributing
Here is documented my journey and contributions to various open-source projects
## Summary
- [Clippy](#clippy)
- [Lambdo](#lambdo)
- [Lumper](#lumper)
- [scala-microservice-scaffold](#scala-microservice-scaffold)
- [GitOps Demo](#gitops-demo)
- [TES](#tes)
- [Temperature aggregator](#temperature-aggregator)


## [Clippy](https://github.com/rust-lang/rust-clippy)
### What is it?
Rust Clippy is a collection of lints for the Rust programming language, aimed at catching common mistakes and improving code quality. 
It features over 700 lints divided into categories such as correctness, style, complexity, and performance, with adjustable lint levels. Clippy is known as one of the most important tools of the Rust ecosystem.
### Stack
- Rust
### What did I do?
I was able to contribute to this project by:
- [Discussing about some issues](https://github.com/rust-lang/rust-clippy/issues/12035)
- [Adding a new feature](https://github.com/rust-lang/rust-clippy/pull/12190) (This PR was never merged because we judged that the feature was not necessary, but it was a good experience to work on it)
- Discussing with the community on [Zulip](https://rust-lang.zulipchat.com/#narrow/stream/257328-clippy) 


## [Lambdo](https://github.com/faast-rt/lambdo)
### What is it?
faast-rt/lambdo is a serverless runtime developed in Rust. It aims to offer a straightforward and efficient method for executing code in any language.  
Based on the [Lumper](#lumper) project, it allows to run code in a totally secure and isolated way.  
One of its features is to be able to generate a runtime for any language, by providing a Docker image containing the language runtime and a simple configuration file.
### Stack
- Rust
- [Lumper](#lumper)
### What did I do?
On Lambdo, I was able to contribute by:
- Defining and implementing the Rest API
- Work on the communication process with the VM agent (using my work done on Lumper)
- [Create tests to ensure the proper functioning of the API](https://github.com/faast-rt/lambdo/pull/20)


## [Lumper](https://github.com/do4-2022/lumper)
### What is it?
The Lumper project is focused on providing a basic Rust-based VMM (Virtual Machine Monitor). It's designed as a straightforward tool to run VM (Virtual Machine), taking profit of Rust's performance and safety features. 
### Stack
- Rust
### What did I do?
On this project, I mainly worked the communication process:  
- With the VM agent through a serial port 
- With the host through a Unix socket
Thanks to this, we were able to send the code execution request to the VM agent, and then retrieve the result from the host.


## [scala-microservice-scaffold](https://github.com/do4-2022/scala-microservice-scaffold.g8)
### What is it?
This project provides a Giter8 template for scaffolding Scala microservice applications that aims to help developers quickly set up and start such applications.  
It allows users to easily start their projects with a pre-configured environment, including: 
- A basic project structure
- A build tool (sbt)
- A message queue (RabbitMQ by default)
- A database (PostgreSQL by default)
- An HTTP server
- The required terraform files to deploy the application
### Stack
- Scala
- sbt
- RabbitMQ
- PostgreSQL
- Terraform
### What did I do?
I was one of the core contributors on this project, and was responsible for: 
- Defining the global structure of the project
- The message queue connector implementation
- Reviewing and merging pull requests


## [GitOps Demo](https://github.com/Roxxas96/gitops-demo)
### What is it?
This repository showcases a demo application designed to illustrate the GitOps framework. This project serves as an example of how to implement GitOps principles, which involve using Git as a single source of truth for declarative infrastructure and applications. With a focus on automation and CI/CD practices, it demonstrates how changes in a Git repository can automatically trigger updates in the application's infrastructure and deployment processes. 
### Stack
- Kubernetes
- Helm
- TypeScript
- React
- Postgres
### What did I do?
As a contributor to this project, I was able to:
- [Add a new feature for 'clearing' the database](https://github.com/Roxxas96/gitops-demo/commit/c52191f7b6b509cb666e3816a8d93f1cecc34da3)
- [Fix the deployment of the application by upgrading the helm chart's version](https://github.com/Roxxas96/gitops-demo/commit/858c44fd94afb435ea18abf61070f25d499b3f3b)


## [TES](https://github.com/alexis-langlet/TES)
### What is it?
The TES (also known as "Time Entry Sender"), is a tool designed to simplify the process of creating time entries on Redmine. It's specifically tailored to consume Redmine's API and facilitates the management of time entries by allowing users to input their details through a user-friendly interface. The project aims to streamline the time entry creation process, making it more efficient to create redundant time entries. 
### Stack
- Go
- Vue.js
### What did I do?
I am currently the sole contributor to this project, but contributions are very welcome. 
I was able to create a basic structure for the project, and implement the following features:
- The user interface
- The Redmine API connector
- The time entry creation process
- checking for public holidays
- choice of credentials (API token or username/password)


## [Temperature aggregator](https://github.com/alexis-langlet/temperature-aggregator)
### What is it?
This project was mainly intended to demonstrate different ways of testing in Rust. It is basically an API that collect temperature data from different sources, process and aggregate them, and then expose the result through an HTTP API.
### Stack
- Rust
### What did I do?
I'm currently the only contributor on this project. As such, I was responsible for:
- The global structure of the project
- The implementation of the temperature sources
- The implementation of the temperature aggregator
- The implementation of the HTTP API
- The implementation of the tests
