🌍 Geolocation Data Management in ServiceNow
📌 Project Overview

This project demonstrates ServiceNow full-stack development by building a custom application that integrates a Service Portal UI, a custom table, and an external REST API for IP-based geolocation lookups.
It automates the process of retrieving, storing, and displaying geolocation information for any given IP address — eliminating manual lookups and providing a centralized data repository for analysis and reporting.


⚙️ Features
🔹 Custom Table: Stores detailed IP geolocation data.
🔹 REST API Integration: Fetches data from ipgeolocation.io
🔹 Server-Side Script: Handles API calls, parses nested JSON, and maps fields.
🔹 Service Portal Widget: Provides an input box, button, and dynamic results table.
🔹 Automated Record Creation: Each lookup is persisted in the database.


🛠️ Implementation Steps
1. Create Custom Table
Navigate to: System Definition → Tables → New
Define fields for IP, country, city, latitude, longitude, timezone, ISP, etc.

2. Build Widget
Go to System UI → Widgets → New
Add:
HTML Template → Input + Button + Display Table
Server Script → Outbound API call & response parsing
Client Script → Trigger server script on button click

3. Add to Portal Page
Navigate: Service Portal → Pages → New
Use the Designer to add a container/grid
drag & drop your custom widget


🚀 Usage
Navigate to the ServiceNow instance → /sp?id=ip_geolocation_lookup
Enter a valid IP address
Click Lookup IP Address
View live results on the portal + stored record in the database


🧪 Testing
Verified results from multiple IP addresses
Ensured records were successfully stored in the custom table
Confirmed UI dynamically updates after each lookup


Conclusion
The Geolocation Data Management Application highlights:
ServiceNow UI design
API integration with external services
Robust backend scripting
Efficient database persistence
API integration with external services
Robust backend scripting

Efficient database persistence
