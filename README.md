# Docker-Kubernetes
* Containers, Docker, Docker Compose
* Docker Registry
* Kubernetes
    * Pods
    * Workloads
    * Services
    * Updates
    * Storage
    * App Settings
    * Observability 
    * Scaling

## Microservices Architecture
A Variant of the service-oriented architecture (SOA) structural style arranges an application as a collection of loosely couped services. 

In a microservices architecture, service-oriented services are fine-grained and the protocols are lightweight.

## Monolithic Architecture
* Built as a single unit
* Deployed as a single unit
* Duplicated on each server

## Microservices 
* Segregates functionality into smaller seperate services each with a single reponsibility. 
* Scales out by deploying each service independently.
* Loosely coupled
* Enable autonomous development by different teams, languages and platforms. 
* Can be written by smaller teams. 
* Each microservice can own it's own data/database.

## From Monolith to Microservices
* Break your application/system in small units. 
* Use the strangler pattern.

## Microservices - Benefits
* Improved fault isolation
* Eliminate vendor or technology lock-in
* Ease of understanding
* Smaller and faster Deployments
* Scalability

## Microservices - Drawbacks
* Complexity is added to resolve complexity issues
    * Is your team trained, ready and has made POCs?
    * Don't start with a complex infrastructure. 
* Testing may appear simpler but is it?
* Deployment may appear simpler but is it? 
    * Hard to do with multiple teams
    * One microservice update can impact many mircoservices.
* Multiple databases?
* Latency issues
* Transient errors
* Multiple point of failures
* How about security?

## Cloud Native
* Within a short time, cloud native has become a driving trend in the software industry.
    * It's a new way to think about building comple systems.
    * Takes full advantage of modern software development practices, technologies, and cloud infrastructure.
    * Widely popular in the open source communities. 

## Cloud Native Concepts
