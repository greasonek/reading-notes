# Class 13 Reading Notes

## Basics of CRUD

- **C**REATE - ex) adoption site - animal's personal page - want to make an appointment for a playdate, so complete appointment form (those inputs correlate to the model table in the database), submit data, POST request is sent to API for playdate to be stored in database

- **R**EAD - want to see all confirmed playdates, use GET request to view scheduled appointments without making changes to data stored on API

- **U**PDATE** - want to change appointment date, use PUT, replaces current data of targeted resource (dog whos playdate want to change, the id in the route is how the resource is targeted to ensure only update specified appointment

- **D**ELETE - decided to adopt the dog so need to cancel the playdate, use DELETE  to cancel targeted appointment (use the specific id)

1. Which HTTP method would you use to update a record through an API?

- UPDATE (PUT)

2. Which REST methods require an ID parameter?

- update and delete

## Speed Coding

1. What’s the relationship between REST and CRUD?

- style for creating APIs communicating via HTTP protocol, CRUD is behind the scenes data manipulation via data operations <a href ="https://www.crowdstrike.com/cybersecurity-101/observability/crud-vs-rest/#:~:text=REpresentational%20State%20Transfer%E2%80%94or%20REST,short%E2%80%94run%20against%20backend%20databases.">Source</a>

2. If you had to describe the process of creating a RESTful API in 5 steps, what would they be?

- get all, get one, create one, udpate one, delete one
