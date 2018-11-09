# Microsoft SQL Server (Linux) Kubernetes deployment config
---

This repo contains a Kubernetes deployment code for Microsoft SQL Server (Linux based). <br>
It will setup a staging environment;
- namespace ""
- pv "create a nfs mount point for the pvc"
- pvc "use the pv and maps it inside the container to /var/opt/mssql"
- svc "exports the sql port to a random NodePort"
- deploy "the deployment code to run the MS SQL container"

## TODO;
- check if container runs as a non-root user
  - it runs as root :-(
- able to connect with the mssql studio tool
  - yup it works!
- create a cluster
