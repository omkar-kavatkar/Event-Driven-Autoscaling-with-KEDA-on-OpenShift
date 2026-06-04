# Event-Driven-Autoscaling-with-KEDA-on-OpenShift
## Overview

This project demonstrates event-driven autoscaling of an application on Red Hat OpenShift using KEDA (Kubernetes Event-Driven Autoscaler), Prometheus metrics, and OpenShift User Workload Monitoring.

The application exposes Prometheus metrics through a /metrics endpoint. KEDA monitors HTTP request metrics from Prometheus and automatically scales application pods based on traffic volume.

## Highlights

- Deployed a Prometheus-instrumented application on Red Hat OpenShift.
- Exposed application metrics through the `/metrics` endpoint.
- Configured ServiceMonitor for Prometheus metric scraping.
- Enabled OpenShift User Workload Monitoring.
- Installed and configured KEDA (Custom Metrics Autoscaler).
- Integrated KEDA with Prometheus and Thanos Querier.
- Implemented HTTP request-based autoscaling using PromQL queries.
- Configured TriggerAuthentication for secure metric access.
- Performed load testing using ApacheBench (ab).
- Validated automatic scale-out from 1 to 10 pods under heavy traffic.
- Verified automatic scale-in back to the minimum replica count after traffic reduction.
- Troubleshot ServiceMonitor, Prometheus scraping, authentication, and custom metrics scaling issues.

## Implementation Steps
- Deploy Prometheus Instrumented Application
- Expose Metrics using Service
- Configure ServiceMonitor
- Enable User Workload Monitoring
- Install KEDA Operator
- Configure TriggerAuthentication
- Create Prometheus-based ScaledObject
- Generate Traffic using ApacheBench
- Validate Scale-Out and Scale-In
