# Customizing Fluentd for GKE Sample Code

This is the sample code for customizing fluentd in Google Kubernetes Engine (GKE). The tutorial explains how to run a custom fluentd daemonset inside GKE that sends logs to Google Cloud Logging.

## Overview

The repository contains:
* a convenience script that creates a GKE cluster with logging disabled (create-cluster.sh)
* Manifests for deploying a test logging program and the fluentd daemonset in Kubernetes
* The test logging program source and Dockerfile in test-logger

## Contact Us

Please use [issue tracker](https://github.com/GoogleCloudPlatform/kubernetes-engine-customize-fluentd/issues)
on GitHub to report any bugs, comments or questions regarding SDK development.

We welcome all usage-related questions on [Stack Overflow](http://stackoverflow.com/questions/tagged/google-customizing-fluentd-in-kubernetes-engine)
tagged with `google-cloud-kubernetes-engine`.

## Instructions
1. Open this repo in Cloud Shell with the below button 
<p>
  <a href="https://ssh.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https://github.com/GoogleCloudPlatform/kubernetes-engine-customize-fluentd.git"><img alt="Open in Cloud Shell" src ="https://gstatic.com/cloudssh/images/open-btn.svg"></a>
</p>
2. Set project with the command replacing VALUE for your project

```
 gcloud config set project VALUE
```

3. Run the create-cluster.sh script to create a test cluster on GKE

```
./create-cluster.sh
```

4. Run the test logger, fluentd configmap, and fluentd daemonset

```
kubectl apply -f kubernetes/test-logger.yaml
kubectl apply -f kubernetes/fluentd-configmap.yaml
kubectl apply -f kubernetes/fluentd-daemonset.yaml
```

## More Information

* [Google Cloud Kubernetes Engine](https://cloud.google.com/kubernetes-engine/docs/)
* [Kubernetes](https://kubernetes.io/)
* [Fluentd](https://docs.fluentd.org/articles/quickstart)
