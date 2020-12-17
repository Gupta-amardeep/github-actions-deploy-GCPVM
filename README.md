# github-actions-deploy-GCPVM

Deploy a VM to GCP via github actions:
  This .github/workflows/deploy-vm.yml will create a new VM in GCP using the github runners
  on ubuntu machine by installing GCLOUD SDK connecting using service account and Google
  project Id stored as repo secrets and running gcloud compute instances create command.

Need:
  GCP_PROJECT_ID stire in repo secrest
  GCP_JSON_SERVICE_ACCOUNT json key store in repo secrets
  
Functionality:
  Developer need to create new branch in order to create a new VM everytime
  as we are using VM name according to branch name only
