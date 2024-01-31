# Cloud Storage Triggered Cloud function Demo

Sample that shows how to trigger a cloud Function when a file is uploaded to Cloud storage.

## Deploy Instruction
```
gcloud functions deploy storage_demo \
--runtime nodejs18 \
--entry-point fileData \
--trigger-event google.storage.object.finalize \
--trigger-resource sp24-cit41200-lluu-demo-bucket

```