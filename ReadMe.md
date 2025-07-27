## ✅ OpenShift-v4.12-Baremetal AirGapped Environment.

### ✅  Technical Implementation

#### ✅  Environment Setup

- Network Infromation
- Network Service
- Load Balancer Config Details
- Internet Access
- Storage Information
- Red Hat OpenShift Container Platform 4 - Logical HA Architecture

#### ✅  Configuring HA Node. 

1. Installation Haproxy Required Packages.
1. Configure & Setup HAproxy.
1. Start and Enable Haproxy.
1. Disable firewall & Selinux. 
1. Check HA status. 


#### ✅  Configuring Registry Node.

2.1. Prerequisites node validation. 

- Operating System Details
- Block Device (Hard Disk) Details
- Network Configuration
- Route and Default Gateway Details
- Enabling Repositories

#### ✅ Configuration DNS Setup.

- Install DNS Package. 
- Configure DNS 
- Create Zones 
- nslookup domain

#### ✅ Configuration Chrony. 

- Install Chrony Package. 
- Configure Chrony 
- Checking synchronize time.


#### ✅ Quay Registry Configuration. 
 
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


#### ✅  Mirror OCP 4.18 Images to Quay Mirror Registry

- Download and Install oc-mirror cli command line tool to use the plugin to download images.
- Mirror the version images to the internal container registry
- Create the ImageSetConfiguration with the cluster version and redhat-operator index image
- Listing Operators after pushed in Quay registry.

#### ✅ Installing a OpenShift Cluster in a Disconnected Network on Baremetal Machines

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


#### ✅  User Authentication 

- Configuring an HTPasswd identity provider


#### ✅  Backup ETCD 

- Encrypting the ETCD data
- Backing Up ETCD data

#### ✅ Removing the kubeadmin user

#### ✅  Future Cluster OpenShift version upgrades
