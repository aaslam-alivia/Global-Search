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

## Request

```json
{
    "searchField": {
        "searchTerm": "",
        "filterActive": false
    },
    "filters": [
        {
            "filterType": "Section",
            "filterValue": "All",
            "configurableOptions": [
                "Manual Case",
                "Case within an Initiative",
                "Case Notes",
                "Attachments",
                "Brief and Summary",
                "Involved Parties",
                "Claims",
                "Correspondence",
                "Findings",
                "Admin Actions",
                "Referrals",
                "Reports",
                "Financials",
                "Data Request",
                "Non-case"
            ]
        },
        {
            "filterType": "Case Stage",
            "filterValue": "All",
            "configurableOptions": [
                // List of all valid stages here
            ]
        },
        {
            "filterType": "Case Assignee",
            "filterValue": "All",
            "configurableOptions": [
                // List of all assignee here 
            ]
        {
            "filterType": "Claim Dates",
            "filters": [
                {
                    "dateField": "Adjudication Date",
                    "fromDate": "",
                    "toDate": ""
                },
                {
                    "dateField": "Invoice Date",
                    "fromDate": "",
                    "toDate": ""
                },
                {
                    "dateField": "Member DOB",
                    "fromDate": "",
                    "toDate": ""
                },
                {
                    "dateField": "Member DOD",
                    "fromDate": "",
                    "toDate": ""
                },
                {
                    "dateField": "Paid Date",
                    "fromDate": "",
                    "toDate": ""
                },
                {
                    "dateField": "Received Date",
                    "fromDate": "",
                    "toDate": ""
                },
                {
                    "dateField": "Service From Date",
                    "fromDate": "",
                    "toDate": ""
                }
            ]
        },
        {
            "filterType": "Case Action Dates",
            "filters": [
                {
                    "dateField": "Case Transition Date",
                    "fromDate": "",
                    "toDate": ""
                },
                {
                    "dateField": "Intake Date",
                    "fromDate": "",
                    "toDate": ""
                }
            ]
        },
        {
            "filterType": "Non-Case Action Dates",
            "filters": [
                {
                    "dateField": "Last Updated Date",
                    "fromDate": "",
                    "toDate": ""
                },
                {
                    "dateField": "Creation Date",
                    "fromDate": "",
                    "toDate": ""
                }
            ]
        },
        {
            "filterType": "Data Request Action Dates",
            "filters": [
                {
                    "dateField": "Resubmitted Date",
                    "fromDate": "",
                    "toDate": ""
                },
                {
                    "dateField": "Submitted Date",
                    "fromDate": "",
                    "toDate": ""
                }
            ]
        }
    }
}
```

