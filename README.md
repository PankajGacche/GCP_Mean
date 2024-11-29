# ResumeAI

## Overview


The project is a MEAN project and uses node version 18.

## Step 1: Set Up Google Cloud Shell Environment:
- Go to the GCP console: https://console.cloud.google.com

![alt text](ReadMe_Images/image_.png)

- Click on the terminal icon (Google Cloud Shell) at the top-right corner:

![alt text](ReadMe_Images/image_1.png)

## 2. Set the GCP project:

- gcloud config set project [PROJECT_ID]

![alt text](ReadMe_Images/image_2.png)

![alt text](ReadMe_Images/image_3.png)

## 3. Enable required APIs: Enable the Google Kubernetes Engine (GKE) and Google 
- Container Registry (GCR) APIs: gcloud services enable container.googleapis.com
- gcloud services enable containerregistry.googleapis.com

![alt text](ReadMe_Images/image_4.png)

- Step 2: Create a GKE Cluster:
- Create the GKE cluster: Run the following command in Cloud Shell to create a 3-node GKE cluster in the specified zone: 

gcloud container clusters create mern-cluster --zone us-central1-a --num-nodes=3

![alt text](ReadMe_Images/image_5.png)
![alt text](ReadMe_Images/image_6.png)

## 2. Get cluster credentials: Fetch the credentials for your newly created cluster:
gcloud container clusters get-credentials mern-cluster --zone us-central1-c

![alt text](ReadMe_Images/image_7.png)

## Step 3: Clone the MEAN Application Repository:
Clone the Sample MERN application: In Cloud Shell, clone the GitHub repository:

![alt text](ReadMe_Images/image_8.png)

## Step 4: Build and Push Docker ReadMe_Images/images to Google Container Registry (GCR)

Authenticate with GCR:

gcloud auth configure-docker
![alt text](ReadMe_Images/image_9.png)

- Created pipeline on jenkins server.
![alt text](ReadMe_Images/image-9.png)
![alt text](ReadMe_Images/image-10.png)
![alt text](ReadMe_Images/image-11.png)
![alt text](ReadMe_Images/image-12.png)

- Created jenkins file and push to github repository.
![alt text](ReadMe_Images/image-13.png)
![alt text](ReadMe_Images/image-14.png)
![alt text](ReadMe_Images/image-15.png)
![alt text](ReadMe_Images/image-16.png)
![alt text](ReadMe_Images/image-17.png)

- Run jenkins pipeline.
![alt text](ReadMe_Images/image-19.png)
![alt text](ReadMe_Images/image-20.png)
![alt text](ReadMe_Images/image-21.png)
![alt text](ReadMe_Images/image-22.png)

- Build images via jenkins file and pushed to ECR.
![alt text](ReadMe_Images/image-23.png)
![alt text](ReadMe_Images/image-24.png)

- Deploying mean application using Minikube.
![alt text](ReadMe_Images/image-25.png)

- Login AWS account via cmd.
![alt text](ReadMe_Images/image-26.png)

- Apply .yaml files on minikube cluser and deployed application successfully.
![alt text](ReadMe_Images/image-27.png)
![alt text](ReadMe_Images/image-28.png)
![alt text](ReadMe_Images/image-29.png)

- Now deploying mean application using Eks.
![alt text](ReadMe_Images/image-30.png)
![alt text](ReadMe_Images/image-31.png)
![alt text](ReadMe_Images/image-32.png)

- Apply .yaml files on Eks cluser and deployed application successfully.
![alt text](ReadMe_Images/image-33.png)
![alt text](ReadMe_Images/image-34.png)
![alt text](ReadMe_Images/image-35.png)
![alt text](ReadMe_Images/image-36.png)
![alt text](ReadMe_Images/image-37.png)

- Verified deployment created on Eks cluster.
![alt text](ReadMe_Images/image-38.png)
![alt text](ReadMe_Images/image-39.png)
![alt text](ReadMe_Images/image-40.png)



