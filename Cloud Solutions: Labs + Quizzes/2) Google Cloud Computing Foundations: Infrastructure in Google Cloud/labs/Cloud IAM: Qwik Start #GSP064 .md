# GSP064
[![](https://github.com/CodingWithHardik/CodingWithHardik/blob/main/img/subscribe_button.png)](https://www.youtube.com/@CloudHustlers)
## Login with username 1
## Run in cloudshell
```cmd
export USERNAME2=
```
```cmd
touch sample.txt
gsutil mb gs://$DEVSHELL_PROJECT_ID
gsutil cp sample.txt gs://$DEVSHELL_PROJECT_ID
gcloud projects remove-iam-policy-binding $DEVSHELL_PROJECT_ID --member="user:$USERNAME2" --role="roles/viewer"
gcloud projects add-iam-policy-binding $DEVSHELL_PROJECT_ID --member="user:$USERNAME2" --role="roles/storage.objectViewer"
```
