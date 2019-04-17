# Customizing Fluentd for GKE Sample Code

This is the sample code for customizing fluentd in Google Kubernetes Engine. The tutorial explains how to run a custom fluentd daemonset inside of GKE that sends logs to StackDriver.

## Overview

The repository contains:
* a convenience script that creates a gke cluster with logging disabled
* kubernetes manifests for deploying a test logging program and the fluentd daemonset in kubernetes/
* The test logging program source and dockerfile in test-logger

## Contact Us

Please use [issue tracker](https://github.com/GoogleCloudPlatform/kubernetes-engine-customize-fluentd/issues)
on GitHub to report any bugs, comments or questions regarding SDK development.

We welcome all usage-related questions on [Stack Overflow](http://stackoverflow.com/questions/tagged/google-customizing-fluentd-in-kubernetes-engine)
tagged with `google-cloud-kubernetes-engine`.

## More Information

* [Google Cloud Kubernetes Engine](https://cloud.google.com/kubernetes-engine/docs/)
* [Kubernetes](https://kubernetes.io/)
* [Fluentd](https://docs.fluentd.org/articles/quickstart)
