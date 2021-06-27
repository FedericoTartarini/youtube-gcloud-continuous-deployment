gcloud builds submit --tag gcr.io/<Project-Name>/<AppName>  --project=<Project-Name>

gcloud run deploy <AppName> --image gcr.io/<Project-Name>/<AppName> --platform managed  --project=<Project-Name> --allow-unauthenticated --region us-east1

gcloud iam service-accounts list --project=<Project-Name>

gcloud iam service-accounts keys create ./keys.json --iam-account email@address

gcloud auth activate-service-account --key-file=keys.json