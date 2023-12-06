# hcp-stack-platform

This repo contains the foundational platform resources (HCP Vault, HCP Boundary, HCP Consul, ..) to be used by further workloads. 

The final workload/demo is stacked upon 2 layers.

1st layer provides the required **platform** environment (this repo) 

2nd layer provides and configure the required **platform/services** and the the final **workload**


This methodology is alligned with the so called platform engineering approach. It's highly scalable and secure by its segregation of duty approach. An application team is able to maintain their code base without affecting any other platform or platform/service. Even a shared platform like Vault is usually hosting many platform/services for many different workloads. We lower the risk of an outage through fine grained access control and thus limiting the blast radius. I may separate platform/services and workload in a future iteration.      

