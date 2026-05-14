---
sidebar: 2025_sidebar.html
---


# RAGTIME Search API

Based on the positive feedback we have received at NeuCLIR Report Generation Pilot last year, we provide a search endpoint using [Qwen3 8B Embedding](https://huggingface.co/Qwen/Qwen3-Embedding-8B) using a FAISS index for participants if you do not want to stand up a search engine by yourself. 
The endpoint is powered by [RoutIR](https://github.com/hltcoe/routir). 

Please register at TREC to get the URL to the endpoint. 

## Search

You can use the following HTTP POST request to retrieve documents based on your query. 

```bash
curl -X POST https://get.url.from.trec/pipeline -H "Content-Type: application/json" -d '{
    "pipeline": "ragtime2%20",
    "collection": "ragtime2",
    "query": "your query"
}'
```

Here `ragtime2` is an alias for the pipeline `{zho%25, spa%25, rus%25, eng%25}ScoreFusion`. If you want to retrieve in a single language, you can use one of the languages alone in the `pipeline` field. Please see the documentation of `RoutIR` for more information. 

If you are working with the NeuCLIR data for development, you can replace the pipeline with `ragtime1` to retrieve documents in RAGTIME 2025 languages (i.e., Chinese, Arabic, Russian and English), which is an alias for the pipeline `{zho%25, arb%25, rus%25, eng%25}ScoreFusion`. 

## Get Document Content

You can retrieve the document content also from the search endpoint by using the API `/content`. 
For example, 

```bash
curl -X POST https://get.url.from.trec/content -H "Content-Type: application/json" -d '{
    "collection": "ragtime2",
    "id": "01f01b3d-89c7-4f97-9d14-bd2dcdff190b"
}'
```

## Contact

Please send an email to us if you have any question at [ragtime-organizers@googlegroups.com](ragtime-organizers@googlegroups.com) or at the TREC Slack. 