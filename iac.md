I would use terraform to provision the infrastruture needed on Google cloud
- Redis (memory store): each service would have its own redis instance
- Cloud SQL (Microsoft SQL server): each service would have its own DB instance 
- Cloud Firestore (NoSQL DB): each service would have its own DB instance
- Kubernetes Cluster - multi environment cluster(dev, staging and production)
- Google container registry
- Google storage bucket
- VPC
- Firewall

