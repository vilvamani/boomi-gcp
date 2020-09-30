# boomi-gcp

You can list the active account name with this command:
```
gcloud auth list
```

You can list the project ID with this command:
```
gcloud config list project
```

Start a new session in Cloud Shell and run the following command to set your default compute zone to us-central1-a:
```
gcloud config set compute/zone us-central1-a
```

```
git clone https://github.com/vilvamani/boomi-gcp.git
```

```
gcloud deployment-manager deployments create gcpnetwork --config=config.yaml
```
where gcpnetwork is the name of the deployment.

To delete the deployment, run the below command from the cloned folder:

```
gcloud deployment-manager deployments delete gcpnetwork
```
