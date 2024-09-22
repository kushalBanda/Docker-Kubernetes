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
### Speed and Agility
* Among many things, cloud Native is about speed and agility.
* Users want...
    * Instantaneous responsiveness 
    * Up-to-the minute features
    * No downtime

* The business wants...
    * Acceralerated innovation 
    * Rapid releases of features to meet disruption from competitors
    * Increased confidence - stability/performance


## Application Architecture
* Clean Code
* Domain Driven Design
* Microservices Principles
* Kubernetes Patterns

## Cloud Native Trail Map
1. Containerization (Docker)
2. CI/CD (argo)
3. Orchestration & Application Definition (Kubernetes) & (Helm)
4. Observability & Analysis (Prometheus, fluentd, Jaeger and Open Tracking)
5. Service Proxy, Discovery, & Mesh (envoy, CoreDNS and LINKERD)
6. Network, Policy and Security (CNI, Open Policy Agent and Falco)
7. Distributed Database & Storage (Vitess, Rook, etcd and KV)
8. Streaming & Messaging (gRPC and NATS)
9. Container registry * Runtime
10. Software Distribution

## What is a Container?
* A unit of software/deployment
    * Code
    * Runtime
    * System Tools
    * System libraries

## Why Containers?
* Move faster by deploying smaller units.
* Use fewer resources
* Fit more into the same host
* Faster automation
* Portability
* Isolation

## Notes about Containers 
* Containers are made of layers
* Container Registry
    * Centralized container repository
    * Think Github for containers
* Orchestrator
    * Manage
        * Infrastructure
        * Containers
        * Deployment
        * Scaling
        * Failover
        * Health monitoring
        * App upgrades, Zero-Downtime deployments
    * Install your own
        * Kubernetes, Swarm, Service Fabric
    * Orchestrators as a service
        * Azure Kubernetes Service, Service Fabric

## What is Docker?
* An open source container runtime
* Mac, Windows and Linux Support
* Command line tool
* "Dockerfile" file format for building container images. 

## Docker CLI Cheat Sheet Management
``` bash
docker info
```
* Display system information

```bash
docker version
```
* Display the system's version

```bash
docker login   
```
* Log in to a Docker registry

``` bash
docker pull [imageName]
```
* Pull an image from a registry

``` bash
docker run [imageName]
```
* Run Containers

``` bash
docker run -d [imageName]
```
* Detached model

``` bash
docker start [containerName]
```
* Start Stop containers

``` bash
docker ps
```
* List running containers

``` bash
docker ps -a
```
* List running and stopped containers

``` bash
docker stop [containerName]
```
* Stop containers

``` bash
docker kill [containerName]
```
* Kill containers

``` bash
docker image inspect [imageName]
```
* Get image info