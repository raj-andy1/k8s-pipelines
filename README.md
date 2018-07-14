### Usage

#### Required for persistant volumes:

```
gcloud compute disks create --size 50GB pipelines-pfc-artifactory --project YOUR_GCLOUD_PROJECT --zone YOUR_K8S_ZONE

gcloud compute disks create --size 50GB pipelines-pfc-mysql --project YOUR_GCLOUD_PROJECT --zone YOUR_K8S_ZONE
```

#### Installation:

Put this in a kubernetes cluster by cloning the project.

From the project directory first run `kubectl create namespace pfc`

and then run `kubectl create -R -f .`
