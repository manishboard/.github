# Project Plan

## Steps

1. **Push Backend on DockerHub**
   - Create a Docker image for the backend.
   - Push the image to DockerHub as a public repository.

2. **Run Backend on Local K3s**
   - Pull the backend image from DockerHub.
   - Deploy and run the backend service on a local K3s cluster.

3. **Deploy Frontend on GitHub Pages**
   - Host the frontend on GitHub Pages.
   - Configure the frontend to communicate with the backend running on the local K3s cluster.

4. **Create an EKS Cluster**
   - Set up an Amazon EKS cluster for deploying applications.

5. **Run Pods on EKS**
   - Deploy backend and other necessary services as pods.
   - Ensure pods pull the backend image from the public DockerHub repository.

6. **Push Image to ECR and Use in Pods**
   - Push the backend image to AWS Elastic Container Registry (ECR).
   - Update deployments to use the ECR image instead of DockerHub.

7. **Create a Helm Chart**
   - Develop a Helm chart to automate the deployment process.
   - Ensure it manages the entire system, including backend and necessary configurations.
