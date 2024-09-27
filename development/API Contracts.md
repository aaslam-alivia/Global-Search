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
{
  "search": "example search term",
  "searchFilters": [
    {
      "isFilterChanged": true,
      "listFilters": [
        {
          "filterType": "Module",
          "filterValue": [
            "Manual Case",
            "Case within Initiative",
            "Non Case",
            "Data Request"
          ]
        },
        {
          "filterType": "Sub Module",
          "filterValue": [
            "Manual Case",
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
          "filterType": "Case Name",
          "filterValue": []
        },
        {
          "filterType": "Plan Code & Name",
          "filterValue": []
        },
        {
          "filterType": "Assignee",
          "filterValue": []
        },
        {
          "filterType": "Stage",
          "filterValue": []
        },
        {
          "filterType": "Status",
          "filterValue": []
        }
      ],
      "dateFilters": [
        {
          "filterType": "Claim Dates",
          "filterValue": [
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
          "filterValue": [
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
          "filterValue": [
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
          "filterValue": [
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
      ]
    }
  ],
  "gridFilters": [
    {
      "search": {
        "searchField": "anything",
        "isFilterChanged": true,
        "columnFilters": [
          {
            "columnName": "Case",
            "searchField": "case id",
            "direction": "DESCENDING"
          },
          {
            "columnName": "Module",
            "searchField": "module",
            "direction": "DESCENDING"
          },
          {
            "columnName": "Sub Module",
            "searchField": "sub module",
            "direction": "DESCENDING"
          },
          {
            "columnName": "Result",
            "searchField": "search results",
            "direction": "DESCENDING"
          },
          {
            "columnName": "Stage",
            "searchField": "stage",
            "direction": "DESCENDING"
          },
          {
            "columnName": "Assignee",
            "searchField": "assignee",
            "direction": "DESCENDING"
          }
        ]
      }
    }
  ]
}
  
```
