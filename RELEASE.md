# netd releases

## 0.2.1 [backlog]
### Features
### Bug fixs

## 0.2.0
### Features
 * Add network metrics collection
### Bug fixs
 * Fix golint errors

## 0.1.9
### Features
### Bug fixs
 * Reduce Calico CNI's log_level from debug to info, Add MTU=1460 for Calico CNI on GCP
 * Remove version info from init container script.
 * Remove calico_cni_spec_template from netd yaml
 * Enable IPv6 forwarding when Calico CNI is used.

## 0.1.8 [backlog]
### Bug fixs
 * fix reconcile and ipmasq chain bug
 * update comments

## 0.1.7
### Bug fixs
 * Quick fix to avoid unnecessary CNI spec generation. PR#44

## 0.1.6
### Features
 * Add support for generating a Calico CNI Spec.
 * Update netd DaemonSet's updateStrategy to be RollingUpdate and tolerations.
 * Make reconcile interval configurable.
 * Ensure configurations once the controller loop started.
 * Version and config logging.
 * change nodeSelector label to gke instead of k8s
 * update the addonmanager mode to Reconcile
### Bug fixs
 * Update dependency.

## 0.1 - 0.1.5
### Features
 * Multi-Container Architecture, use init container for spec generation.
 * netd infrastructure.
 * Deploy PTP CNI spec.
 * Configure pods with an additional IPv6 address if Direct Path is enabled.
 * Reconcile policy routing implemented by ip, iptables rules and sysctl settings.
