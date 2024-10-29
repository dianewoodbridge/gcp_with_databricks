## The codes works on Databricks using GCP as compute resources.
### Pre-requisite : 
- Create a GCP account and a project.
- Create bucket with data.
- In order to allow the Databrick to read from your GCS bucket, you need to create a GCP Service Account with a proper role (ex. Storage Admin) and add to your cluster.
<ol>
  <li>Go to your project in GCP => IAM & Admin => Service Account => Create Service Account</li>
  <li>Create an account with Storage Admin (or something that gives a storage access) and copy its Principal.</li>
  <li>Add the GCP Service Account Principal to your cluster => Advanced => Google Service Account.</li>
  <li>In your notebook, you can access your objects in GCS by "gs://bucket/path"</li>
</ol>
- You can also add libraries/packages to install under your Compute => Libraries.
