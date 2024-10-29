## The codes work on Databricks using GCP as compute resources.
### Pre-requisite : 
<ul> 
<li>Create a GCP account and a project.</li> 
<li>Create a bucket with data.</li> 
<li>In order to allow the Databrick to read from your GCS bucket, you need to create a GCP Service Account with a proper role (ex. Storage Admin) and add it to your cluster.</li> 
<ol>
  <li>Go to your project in GCP => IAM & Admin => Service Account => Create Service Account</li>
  <li>Create an account with Storage Admin (or something that gives a storage access) and copy its Principal.</li>
  <li>Add the GCP Service Account Principal to your cluster => Advanced => Google Service Account.</li>
  <li>In your notebook, you can access your objects in GCS by "gs://bucket/path"</li>
</ol>
<li>You can also add libraries/packages to install under your Compute => Libraries.</li>
</ul>
