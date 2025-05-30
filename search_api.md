---
sidebar: 2025_sidebar.html
---


# RAGTIME Search API

Based on the positive feedback we have received at NeuCLIR Report Generation Pilot last year, we provide a search endpoint using [PLAID-X](https://github.com/hltcoe/colbert-x) again for participants if you do not want to stand up a search engine by yourself. 
PLAID-X is a very effective MLIR model, which is developed along with teh NeuCLIR track. 

Please register at TREC to get the URL to the endpoint. 

## Search

You can use the following HTTP POST request to retrieve documents based on your query. 

```bash
curl -X POST https://get.url.from.trec/query -H "Content-Type: application/json" -d '{
    "service": "plaidx-ragtime",
    "query": "your query",
    "limit": 10
}'
```

If you are working with the NeuCLIR data for development, you can also search among the NeuCLIR collection by specifying `plaidx-neuclir` in the `service` field. 
You can also specify the language of the documents (only for NeuCLIR) by passing the language code to the `subset` field. 
For example, 

```bash
curl -X POST https://get.url.from.trec/query -H "Content-Type: application/json" -d '{
    "service": "plaidx-neuclir",
    "query": "your query",
    "limit": 100,
    "subset": "fas"
}'
```

## Get Document Content

You can retrieve the document content also from the search endpoint by using the API `/content`. 
For example, 

```bash
curl -X POST https://get.url.from.trec/query -H "Content-Type: application/json" -d '{
    "collection": "neuclir",
    "id": "01f01b3d-89c7-4f97-9d14-bd2dcdff190b"
}'
```

You can put either `neuclir` or `ragtime` to the `collection` field. 

## Contact

Please send an email to us if you have any question at [ragtime-organizers@googlegroups.com](ragtime-organizers@googlegroups.com) or at the TREC Slack. 