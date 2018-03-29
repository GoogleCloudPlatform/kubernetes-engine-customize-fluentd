# Customizing Fluentd for GKE Sample Code

This is the sample code for the Customizing fluentd in Google Kubernetes Engine.  The tutorial explains how to run a custom fluentd daemonset inside of GKE that sends logs to StackDriver. 


## Overview

The repository contains 4 types of artifiacts
1. Deployment manager scripts for creating a container-engine cluster with version 1.7.4 and cloud logging turned off in gke-cluster/
2. kubernetes manifests for deploying a test logging program and the fluentd daemonset in kubernetes/
3. The test logging program source and dockerfile in test-logger/
4. Convenience scripts for speeding up some of the steps in the tutorial


## Contact Us

Please use [issue tracker](https://github.com/GoogleCloudPlatform/container-engine-customize-fluentd/issues)
on GitHub to report any bugs, comments or questions regarding SDK development.

We welcome all usage-related questions on [Stack Overflow](http://stackoverflow.com/questions/tagged/google-customizing-fluentd-in-kubernetes-engine)
tagged with `google-cloud-kubernetes-engine`.

## More Information

* [Google Cloud Container Engine](https://cloud.google.com/container-engine/docs/)
* [Google Cloud Deployment Manager](https://cloud.google.com/deployment-manager/docs/)
* [Kubernetes](https://kubernetes.io/)
* [Fluentd](https://docs.fluentd.org/v0.12/articles/quickstart)
