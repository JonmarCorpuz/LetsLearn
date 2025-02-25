# Kubernetes Engine Overview

The Google Kubernetes Engine is a managed Kubernetes service for containers and container clusters running on GCP

* Uses the Container-Optimized OS (A hardened OS built by Google)
* Multiple clusters can be managed as a group (fleet)
* Allows you to manage multiple microservices within a cluster
* Provides the benefits of using Kubernetes without the administrative overhead
* Provides load balancing across Compute Engine VMs that are deployed in GKE

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/Whitespace.png)

# Kubernetes Engine Container External Deployment Methods

## LoadBalancer

Externally exposes the service using the Cloud Service Provider's load balancer 

## ClusterIP 

Internally exposes the service using the cluster's interal IP address 

## NodePort 

Externally exposes the service using the node's IP address at a static port

## ExternalName 

Externally exposes the service using the value mapped to the value of the externalName field in the DNS server 

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/Whitespace.png)

# Kubernetes Engine Cluster Types

## Single Zone Zonal Cluster

* All nodes within the cluster are running in the same zone

## Multi Zone Zonal Cluster

* Not all nodes within the cluster are running in the same zone

## Regional Cluster

* All nodes within the cluster are running within the same zone whiel having one or more regions are running a replica of the control place

## Alpha Cluster

* An instable cluster that's running with alpha features enabled for testing purposes

## Windows Cluster

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/Whitespace.png)

# Kubernetes Engine Cluster Visibility

## Private Cluster

* A VPC-native cluster where the Master and Worker nodes are only accessible within their private network (All communication done between the two are via private addresses only)
* Nodes only have private IP addresses

## Public Cluster

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/Whitespace.png)

# Kubernetes Engine Cluster Modes

## Standard Cluster 



* Users are responsible for configuring and managing the Nodes
* Follows a pay-per-node model where the customer is charged for the provisioned resources used when their application is running

## Autopilot Cluster 

* Provides a hands-off experience (*GKE will configure and manage the cluster infrastructure*, *GKE will manage VPC-native traffic routing for public and private clusters*, *GKE will use Shielded GKE Nodes*, *GKE manages the nodes, meaning that there are no node pools for you to manage*, *etc.*)
* Reduces your operational costs in running Kubernetes clusters by following a pay-per-pod model
* Uses preconfigured and optimized cluster configurations

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/Whitespace.png)

# Kubernetes Engine Security Features

![](https://github.com/JonmarCorpuz/SecondBrain/blob/main/Assets/Whitespace.png)

# Configure Kubernetes Cluster

## kubeconfig

Configure the kubeconfig file on a cluster
```Bash
gcloud container clusters get-credentials --zone <ZONE> <CLUSTER_NAME>
```
