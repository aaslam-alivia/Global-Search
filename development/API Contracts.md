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

This JSON structure is used to define parameters for a global search in the application.

```json
{
    "ai_workflow_param_data": {
        "ai_workflow_grid_id": "123",
        "ai_workflow_grid_name": "globalSearchAdvanceList",
        "ai_workflow_ds_id": "",
        "ai_workflow_grid_filter_value": "12",
        "ai_workflow_grid_sort_column_name": [
            {}
        ],
        "ai_workflow_grid_filter": [
            {
                "filterType": "Section",
                "filterValue": "All",  // or specific section
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
                "filterValue": "All",  // or specific case stage
                "configurableOptions": [ 
                    // List of all valid stages here
                ]
            },
            {
                "filterType": "Case Assignee",
                "filterValue": "All",  // or specific assignee
                "dynamicOptions": true,
                "onlyUnlockedUsers": true
            },
            {
                "filterType": "Claim Dates",
                "filters": [
                    {
                        "dateField": "Adjudication Date",
                        "fromDate": "", // Required
                        "toDate": "" // Optional
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
                    // Add more date fields as needed
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
        ],
        "searchField": {
            "searchTerm": "",  // The user's search input
            "filterActive": false // Indicates if any filters are set
        }
    },
    "ai_workflow_data_object": {}
}```

