# Build smarter apps with Office365 using the Microsoft Graph (Yina Arenas)

## Opportunity

a unified REST API and comprehensive developer experience for integrating the data and intelligence exposed by Microsoft services.

Stars with data of users in organization 
-> adds documents
-> goes to conversational data
-> calculate insights (important analytics, who the are, what they're doing)

Microsoft Graph is the core whether you're building a standalone web/device app or extesniosn with Office Canvases or Sharepoint integration with Sharepoint pages.

Single endpoint, to access organizational data.
One token
All User

https://graph.microsoft.com

## Microsoft Graph 101

2 core concepts 

### Data

AD Users/Groups members and conversations, Sharepoint Lists/sites, OneDrive Files, Outlook, Excel, OneNote, Planner, Contacts, Directory

Beta: Teams, Insights, Project Rome, InTune, Reports

1) graph.microsoft.com - documentation

2) Graph Explorer - REST endpoint that allows you to query the endpoints and get a JSON object in return. The documentation shows plenty of examples and explains how to utilize the query parameters.

https://graph.microsoft.com/{version}/{resource}/{id}/{property}?{query-parameters}

`/me` endpoint is a shortcut to /users/id

You can query any of the data points you have access to and get a JSON file in return. 

### Capabilities

Open Extensions and Schema extensions

Use $batch - ability to add request to JSON batches and add/chain multiple requests on the single request

v1.0 - only uses work accounts

v2.0 - both work and personal accounts

Create application, add platform, Add permissions for admin consent flows
