# OpenShift-v4.12-Baremetal

## Technical Implementation

## 0. Environment Setup

- Network Infromation
- Network Service
- Load Balancer Config Details
- Internet Access
- Storage Information
- Red Hat OpenShift Container Platform 4 - Logical HA Architecture

## 1. Configuring HA Node. 

1. Installation Haproxy Required Packages.
1. Configure & Setup HAproxy.
1. Start and Enable Haproxy.
1. Disable firewall & Selinux. 
1. Check HA status. 


## 2. Configuring Registry Node.

2.1. Prerequisites node validation. 

- Operating System Details
- Block Device (Hard Disk) Details
- Network Configuration
- Route and Default Gateway Details
- Enabling Repositories

2.2 Configuration DNS Setup.

- Install DNS Package. 
- Configure DNS 
- Create Zones 
- nslookup domain

2.3 Configuration NTP setup. 

- Install NTP Package. 
- Configure NTP 
- Checking synchronize time.


2.4 Quay Registry Configuration. 
 
- Install podman and container-selinux packages for standalone registry
- Check podman and buildah version needed for Quay Mirror Registry as it needs podman version greater than 3.0
- Extract mirror registry. 
- Install the Quay Mirror Registry 
- Certificate pem directory placement
- Quay login testing 
- Extract pull-secret from quay mirror registry
- Online pull secret download and configure serve to quay registry.
- Setting up variables requirements for ocp images
- Downloading and Pushing OCP-Base-Images


2.3. Mirror OCP 4.12 Images to Quay Mirror Registry

- Download and Install oc-mirror cli command line tool to use the plugin to download images.
- Mirror the version images to the internal container registry
- Create the ImageSetConfiguration with the cluster version and redhat-operator index image
- Listing Operators after pushed in Quay registry.

## 3. Installing a OpenShift Cluster in a Disconnected Network on Baremetal Machines


3.1. Installing a OpenShift Cluster Setup.

- Generating an SSH private key and adding it to the agent
- Manually creating the installation configuration file
- Creating the Openshift/Kubernetes manifest
- Install and Configure Apache HTTPD Server
- Openshift 4.12 Bootstrapping
- Openshift Skeleton Deployment

- Create Machine Config Pool for infra nodes
- Move Ingress Controller components to infra nodes
- Moving monitoring components from Worker to Infra labeled nodes
- Deploying Openshift Internal Registry with Persistent Storage
- Configure System Clock Sync with NTP Server
- Configure master nodes system clock sync with NTP server


3.2. Deploying and Configuring Dell Unity XT CSI Driver for presistent block storage.

- Install dell Operators
- Create a new namespace named unity.
- Switch to unity project
- Creating a Secret.
- Creating a Configmap.
- Creating a StorageClass.



## 4. Deploying and Configuring Openshift Logging with Persistent Storage

- Install Cluster Logging Operators
- Install the Cluster Logging Operator
- Create Cluster Logging Instance
- Viewing cluster logs from the Kibana dashboard


## 5. User Authentication 

- Configuring an HTPasswd identity provider


## 6. Configure Namespace/Project based isolation with Network Policy Multitenant Configuration

- Creating default network policies for a new project
- Adding network policy objects to the new project template

## 7. Backup ETCD 

- Encrypting the ETCD data
- Backing Up ETCD data

## 8. Removing the kubeadmin user

## 9. Future Cluster OpenShift version upgrades