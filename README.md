# Event-Driven-Autoscaling-with-KEDA-on-OpenShift
Overview

This project demonstrates event-driven autoscaling of an application on Red Hat OpenShift using KEDA (Kubernetes Event-Driven Autoscaler), Prometheus metrics, and OpenShift User Workload Monitoring.

The application exposes Prometheus metrics through a /metrics endpoint. KEDA monitors HTTP request metrics from Prometheus and automatically scales application pods based on traffic volume.
