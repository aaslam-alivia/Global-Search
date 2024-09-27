# Basic Global Search

## Request 

```json
{
    "search_string": "hel",
    "filters": [
        {
            "recent": []
        },
        {
            "appSection": []
        },
        {
            "assignee": []
        },
        {
            "stage": []
        }
    ],
    "isFilterChanged": false
}
```

# Advance Global Search 

## Request (with search test)

```json
{
    "user": {
        "userId": "12345",
        "orgId": "org1",
        "tenant": "tenantA"
    },
    "search": "test",
    "page": {
        "page": 0,
        "size": 10
    }
}

```

## Request (with search and filter)

```json
    
```
