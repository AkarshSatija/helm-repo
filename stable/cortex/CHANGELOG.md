# Changelog

## master / unreleased

* [ENHANCEMENT] Expose new HTTP API paths for remote-write and Query frontend to nginx #103
* [ENHANCEMENT] Compactor service is no longer created if compactor is disabled. #82
* [ENHANCEMENT] Headless service for alert manager is only enabled when the alert manager is deployed as a stateful set. #91
* [ENHANCEMENT] Improved memcached configuration template, with support for both chunks & block storage caches. #92
* [ENHANCEMENT] Update apiVersion: networking.k8s.io/v1beta1 -> networking.k8s.io/v1 for Kubernetes versions 1.19+  #94
* [BUGFIX] Update repository URL for memcache dependency charts. #96
## 0.2.0 / 2020-10-25

* [FEATURE] Add support for Blocks storage backend of Cortex. #52
* [ENHANCEMENT] Adding dnsResolver option to nginx.config. #28
* [ENHANCEMENT] Supporting externally managed Cortex Config. #31
* [ENHANCEMENT] Enabling NGINX deployment to be optional. #32
* [ENHANCEMENT] Adding option to deploy ingester as StatefulSet. #46
* [ENHANCEMENT] Adding ability to run alertmanager as StatefulSet. #54
* [ENHANCEMENT] Updating README.MD with values.yaml defaults, adding alertmanager paths to nginx. #57
* [BUGFIX] Updating query frontend headless service to publish its address when not ready, to fix issue with queriers not becoming ready due to not finding any frontend addresses. #34
* [BUGFIX] Fixed invalid config template. #40
* [BUGFIX] Correct & add consistent target labels on components. #48
* [BUGFIX] Fix values file duplicate config.storage section of Cortex config. #51
* [BUGFIX] Add GRPC ports to store gateway pods and service. #52
* [BUGFIX] Fix service ports, fix ruler endpoint for configs and alertmanager. #55
