gcloud builds submit --tag gcr.io/<Project-Name>/<AppName>  --project=<Project-Name>

gcloud run deploy <AppName> --image gcr.io/<Project-Name>/<AppName> --platform managed  --project=<Project-Name> --allow-unauthenticated --region us-east1

gcloud iam service-accounts list --project=<Project-Name>

gcloud iam service-accounts keys create ./keys.json --iam-account email@address

gcloud auth activate-service-account --key-file=keys.json

# Useful links
* Paul Craig [blog](https://dev.to/pcraig3/quickstart-continuous-deployment-to-google-cloud-run-using-github-actions-fna)
* GitHub action [deploy-cloudrun](https://github.com/google-github-actions/deploy-cloudrun)
* Cloud Run simple Flask application [tutorial](https://cloud.google.com/run/docs/quickstarts/build-and-deploy/python)
* [Installing Google Cloud SDK](https://cloud.google.com/sdk/docs/install)