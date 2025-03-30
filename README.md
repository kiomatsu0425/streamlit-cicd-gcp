# streamlit-cicd-gcp

uv run streamlit run home.py

# Deploy

```
gcloud run deploy my-app --region "asia-northeast1" --source . \
    --allow-unauthenticated --quiet
```

# Delete

以下だと Cloud Run しか消えない。他にも Artifact Registroy とかもある。

```
gcloud run services delete my-app --region"asia-northeast1"
```
