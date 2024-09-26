# ELK Commands

Run these commands locally or in the ELK environment.

## Get Document Content

Retrieve the content of documents from the specified index:

```bash
curl --location "http://10.64.8.18:9200/attachmentsfiles8f6d5458-5e84-4e93-8bd7-49279eb97e48/_search" \
--header "Content-Type: application/json" \
-u "elastic:Alivia@2024" \
--data '{
    "query": {
        "match_all": {}
    },
    "from": 0,
    "size": 1000
}'

## Get Index Document Count

curl -X GET "http://10.64.8.18:9200/attachmentsfiles8f6d5458-5e84-4e93-8bd7-49279eb97e48/_count" \ -u "elastic:Alivia@2024"

## Search within Index Document

curl --location "http://10.64.8.18:9200/attachmentsfiles8f6d5458-5e84-4e93-8bd7-49279eb97e48/_search" \
--header "Content-Type: application/json" \
-u "elastic:Alivia@2024" \
--data '{
    "query": {
        "match": {
            "attachment.content": "john walk"
        }
    }
}'



