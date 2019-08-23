## Initialize GCP tools

Login into google cloud:
```bash
gcloud auth login
```

Set the default project:
```bash
gcloud config set project YOUR_PROJECT_ID
```

Update Google Cloud components and install kubectl:
```bash
gcloud components update
gcloud components install kubectl
```

Init the default application credentials, only once:
```bash
gcloud auth application-default login
```

Initialize GCP Container Registry (https://cloud.google.com/container-registry/docs/quickstart):
```bash
gcloud auth configure-docker
```
