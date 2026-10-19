# HW-06 - Kubernetes GitOps with Argo CD

## Traefik Installation

Traefik was installed using Helm to expose Argo CD through an Ingress resource.

![Traefik Installation](./utils/image1.png)

---

## Argo CD Ingress Configuration

The Ingress resource uses the hostname `argocd.local` and routes HTTP traffic to the Argo CD server through Traefik.

![Argo CD Ingress](./utils/image2.png)

---

## Argo CD Web Interface

The Argo CD web interface was accessed through:

`http://argocd.local:8080`

![Argo CD Interface](./utils/image3.png)

---

## Application 1 - Nginx

The first Argo CD Application deploys an Nginx container using the manifests stored in `apps/app1`.

- **Application:** `app1-nginx`
- **Image:** `nginx:1.27`
- **Namespace:** `parcial-gffh`
- **Service Port:** `80`

![Nginx Application](./utils/image4.png)

---

## Application 2 - Apache

The second Argo CD Application deploys an Apache HTTP Server container using the manifests stored in `apps/app2`.

- **Application:** `app2-apache`
- **Image:** `httpd:2.4`
- **Namespace:** `parcial-gffh`
- **Service Port:** `80`

![Apache Application](./utils/image5.png)

---

## Synchronization and Health Status

Both applications were synchronized with the GitHub repository and reached the `Healthy` status in Argo CD.

- `app1-nginx`: **Synced / Healthy**
- `app2-apache`: **Synced / Healthy**

![Argo CD Applications Synced and Healthy](./utils/image8.png)

---

## Kubernetes Resources Verification

The Kubernetes pods and services were verified in the `parcial-gffh` namespace. Both application pods reached the `Running` state and were ready.

![Kubernetes Resources](./utils/image9.png)

---
