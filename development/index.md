# Elasticsearch Indices

This project interacts with the following Elasticsearch indices:

- **header**
- **claims**
- **claimsheader**
- **claimsaudit**
- **reporting**
- **correspondence**
- **brief**
- **notes**
- **involvedparties**
- **attachments**
- **findings**
- **administrative_action**
- **referrals**
- **finance**
- **attached-dashboard**
- **attachmentsfiles**
- **member**
- **provider**

## Multi-Index Search

You can perform a search across multiple indices using the following request format:

```bash
POST https://localhost:9200/header,claims,claimsheader,claimsaudit,reporting,correspondence,brief,notes,involvedparties,attachments,findings,administrative_action,referrals,finance,attached-dashboard,attachmentsfiles,member,provider/_search
