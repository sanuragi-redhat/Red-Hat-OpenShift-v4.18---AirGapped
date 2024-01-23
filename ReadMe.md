# OpenShift-v4.12-Baremetal

## Technical Implementation

0. Environment Setup

    1. Node Information
    1. Storage Information
    

1. Creating a mirror registry with mirror registry for Red Hat OpenShift 

    1. Operating System Details
    1. Block Device (Hard Disk) Details
    1. Network Configuration
    1. Route and Default Gateway Details
    1. Enabling Repositories
    1. Install podman and container-selinux packages for standalone registry
    1. Check podman and buildah version needed for Quay Mirror Registry as it needs podman version greater than 3.0
    1. Install the Quay Mirror Registry after the successful install see the below messages
    1. Certificate pem directory placement.
    1. Online pull secret download and configure serve to quay registry.
    1. Setting up variables requirements for ocp images
    1. Downloading and Pushing OCP-Base-Images



2. Mirror OCP 4.12 Images to Quay Mirror Registry

    1. Download and Install oc-mirror cli command line tool to use the plugin to download images.
    1. Mirror the version images to the internal container registry
    1. Create the ImageSetConfiguration with the cluster version and redhat-operator index image
    1. Listing Operators after pushed in Quay registry.
    1. Verify the registry storage size and repositories availability
    1. Verify that, the version information that you mirrored to local registry is matching with quay.io registry



3. Check Bastion Node for all the pre-Installation requirements

    1. Operating System Details
    1. Block Device (Hard Disk) Details
    1. Network Configuration
    1. Route and Default Gateway Details
    1. Enabling Repositories



4. Installing a OpenShift Cluster in a Disconnected Network on Baremetal Machines

    1. Generating an SSH private key and adding it to the agent
    1. Manually creating the installation configuration file
    1. Creating the Openshift/Kubernetes manifest
    1. Install and Configure Apache HTTPD Server
    1. Openshift 4.11 Bootstrapping
    1. Openshift Skeleton Deployment


5. Create Machine Config Pool for infra nodes

6. Move Ingress Controller components to infra nodes

    1. Deploying Openshift Internal Registry with Persistent Storage
    1. Configure System Clock Sync with NTP Server
    1. Configure master nodes system clock sync with NTP server



8. Deploying and Configuring Dell Unity XT CSI Driver for presistent block storage.

    1. Install dell Operators
    1. Create a new namespace named unity.
    1. Switch to unity project
    1. Creating a Secret.
    1. Creating a Configmap.
    1. Creating a StorageClass.

9. Moving monitoring components from Worker to Infra labeled nodes

10. Deploying and Configuring Openshift Logging with Persistent Storage

    1. Install Cluster Logging Operators
    1. Install the Cluster Logging Operator
    1. Create Cluster Logging Instance
    1. Viewing cluster logs from the Kibana dashboard


11. Configuring an HTPasswd identity provider

12. Configure Namespace/Project based isolation with Network Policy Multitenant Configuration

    1. Creating default network policies for a new project
    1. Adding network policy objects to the new project template

13. Backup ETCD 

    1. Encrypting the ETCD data
    1. Backing Up ETCD data

14. Removing the kubeadmin user

15. Future Cluster OpenShift version upgrades