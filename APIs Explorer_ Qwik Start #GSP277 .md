# GSP277
>🚨 [PLEASE SUBSCRIBE OUR CHANNEL CLOUDHUSTLER](https://www.youtube.com/@cloudhustlers) **&** [JOIN OUR COMMUNITY](https://chat.whatsapp.com/KBfUcSleGGEFf2Xvvm8FW3)
## Run in cloudshell
```cmd
export PROJECT_ID=$(gcloud config get-value project)
gsutil mb -p $PROJECT_ID -c regional -l us-central1 gs://$PROJECT_ID-bucket
curl -O https://github.com/siddharth7000/practice/blob/main/sign.jpg
mv sign.jpg demo-image.jpg
gsutil cp demo-image.jpg gs://$PROJECT_ID-bucket/demo-image.jpg
gsutil acl ch -u allUsers:R gs://$PROJECT_ID-bucket/demo-image.jpg
```
