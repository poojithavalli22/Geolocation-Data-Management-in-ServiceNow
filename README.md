🌍 Geolocation Data Management in ServiceNow
📌 Project Overview
This project demonstrates ServiceNow full-stack development by building a custom application that integrates a Service Portal UI, a custom table, and an external REST API for IP-based geolocation lookups.

It automates the process of retrieving, storing, and displaying geolocation information for any given IP address — eliminating manual lookups and providing a centralized data repository for analysis and reporting.

⚙️ Features
Custom Table: Stores detailed IP geolocation data.

REST API Integration: Fetches data from ipgeolocation.io.

Server-Side Script: Handles API calls, parses nested JSON, and maps fields.

Service Portal Widget: Provides an input box, button, and dynamic results table.

Automated Record Creation: Each lookup is persisted in the database.

🛠️ Implementation Steps
1. Create Custom Table
Navigate to: System Definition → Tables → New

Define fields for: IP, country, city, latitude, longitude, timezone, ISP, etc.

2. Build Widget
Go to: System UI → Widgets → New

Add the following components:

HTML Template: Input field, button, and a table to display results.

Server Script: Logic for the outbound API call and response parsing.

Client Script: Code to trigger the server script when the button is clicked.

3. Add to Portal Page
Navigate to: Service Portal → Pages → New

Use the Page Designer to add a container and grid layout.

Drag and drop your custom widget into the container.

🚀 Usage
Navigate to your ServiceNow instance and append the following path to the URL: /sp?id=ip_geolocation_lookup

Enter a valid IP address in the input field.

Click the "Lookup IP Address" button.

View the live results on the portal and see the new record stored in the database.

🧪 Testing
Verified results with multiple public IP addresses.

Ensured records were successfully stored in the custom table.

Confirmed the UI dynamically updates after each lookup.

✅ Conclusion
The Geolocation Data Management Application successfully highlights proficiency in:

ServiceNow UI Design

API Integration with External Services

Robust Backend Scripting

Efficient Database Persistence
