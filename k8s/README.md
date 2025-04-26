# Firecrawl Kubernetes Manifests

This directory contains Kubernetes manifests for deploying Firecrawl.

**Note:** These manifests are generated based on the `docker-compose.yaml` file. You may need to adjust them based on your specific Kubernetes environment and requirements, especially regarding secrets management, ingress configuration, and resource allocation.

## Files

*   `firecrawl-namespace.yaml`: Defines the Kubernetes namespace.
*   `firecrawl-config.yaml`: ConfigMap for non-sensitive configuration.
*   `firecrawl-secret.yaml`: Secret for sensitive data (replace placeholders).
*   `redis-deployment.yaml`: Deployment for Redis.
*   `redis-service.yaml`: Service for Redis.
*   `redis-pvc.yaml`: PersistentVolumeClaim for Redis (optional).
*   `playwright-deployment.yaml`: Deployment for Playwright Service.
*   `playwright-service.yaml`: Service for Playwright Service.
*   `api-deployment.yaml`: Deployment for the API service.
*   `api-service.yaml`: Service for the API service (consider LoadBalancer/NodePort/Ingress).
*   `worker-deployment.yaml`: Deployment for the Worker service. 