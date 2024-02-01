# ECS 193 Advice

Advice points to help you with your capstone project


## Project Accounts:

- When establishing cloud or other online services, use a customer provided name and email address for the account. 
- In the initial stages of development, it's okay to use a personal account for testing out a concept; however, the production environment should only be associated with project accounts.
- This allows you to cleanly step away from the project after it ends and the next developer to quickly access the production resources.


## Data Access:

- Access to data or services might take time due to an approval process, so determine what is required for the project and submit access requests promptly.
- Determine which data fields you will use as key items to connect data between sources.


## Authentication and Authorization:

- Ask about the current identity services used for authentication and authoriziation by the customer.
- Check for an existing roles database or directory service (e.g. Active Directory).
- Map out each app role and it's data access level.
- Consider how new users will be provisioned and roles assigned.
- Determine the role verification process utilized during app usage and what happens if users access content not assigned to them.


## APIs:

- Inquire about existing APIs. The company might already have what you need for the project so you don't have to recreate the wheel.
- Ask which type of API they provide; REST, Websocket, SOAP...
- Most API providers require a developer account to create an app request.
- App requests will be routed to an admin for approval.
- Only request access to what you need for the project.
- For protected API endpoints, ensure you secure your access keys and tokens.
- Know the expiration settings for tokens used in automated processes.


## Web Servers:

- Protect sites with certs and reroute port 80 traffic to port 443.
- Site processes should not be run by root or admin accounts.
- Document each web application and which account they run under and the level of access it has to data and system resources.
- Use input sanitization on all web forms.


## Database Servers:

- Place all database servers behind a firewall and only allow access from required app servers.
- Relational database tables should utilize primary keys.
- Application accounts used for accessing data should have the minimum access required.
- Document each database, application account, stored procedures, backups, and maintenance plans.


## Cloud Data Storage:

- Establish billing alerts to prevent over-charges.
- Periodically check share permissions and collaboration settings.


## Documentation:

- Inform the customer of the location of all documentation.
- Grant the customer access to all code repos.









