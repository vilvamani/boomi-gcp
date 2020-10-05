# boomi-gcp
Network deployment on Google cloud using Deployment Manger

You can list the active account name with this command:
```
gcloud auth list
```

To set your Cloud Platform project in this session use

```
gcloud config set project [PROJECT_ID]
```


You can list the project ID with this command:
```
gcloud config list project
```

Start a new session in Cloud Shell and run the following command to set your default compute zone to us-central1-a:
```
gcloud config set compute/zone us-central1-a
```

Enable the Compute Engine and Deployment Manager APIs, which you will need for this tutorial.

```
gcloud services enable compute.googleapis.com deploymentmanager.googleapis.com  
```

```
git clone https://github.com/vilvamani/boomi-gcp.git && cd boomi-gcp
```

```
gcloud deployment-manager deployments create boomi-quickstart --config=master-config.yaml
```
where gcpnetwork is the name of the deployment.

To delete the deployment, run the below command from the cloned folder:

```
gcloud deployment-manager deployments delete gcpnetwork
```
