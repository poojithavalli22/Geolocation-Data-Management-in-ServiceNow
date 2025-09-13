# 🌍 Geolocation Data Management in ServiceNow

## 📌 Project Overview  
This project demonstrates **ServiceNow full-stack development** by building a custom application that integrates a **Service Portal UI**, a **custom table**, and an **external REST API** for IP-based geolocation lookups.  

It automates the process of retrieving, storing, and displaying geolocation information for any given IP address — eliminating manual lookups and providing a centralized data repository for analysis and reporting.  

---

## ⚙️ Features  
- **Custom Table**: Stores detailed IP geolocation data.  
- **REST API Integration**: Fetches data from [ipgeolocation.io](https://ipgeolocation.io).  
- **Server-Side Script**: Handles API calls, parses nested JSON, and maps fields.  
- **Service Portal Widget**: Provides an input box, button, and dynamic results table.  
- **Automated Record Creation**: Each lookup is persisted in the database.  

---

## 🛠 Implementation Steps  

### 1. Create Custom Table  
- Navigate to: `System Definition → Tables → New`  
- Define fields for: **IP, country, city, latitude, longitude, timezone, ISP**, etc.  

### 2. Build Widget  
- Navigate to: `System UI → Widgets → New`  
- Add the following components:  
  - **HTML Template**: Input field, button, and a table to display results.  
  - **Server Script**: Logic for the outbound API call and response parsing.  
  - **Client Script**: Code to trigger the server script when the button is clicked.  

### 3. Add to Portal Page  
- Navigate to: `Service Portal → Pages → New`  
- Use the **Page Designer** to add a container and grid layout.  
- Drag and drop your custom widget into the container.  

---

## 🚀 Usage  
1. Navigate to your ServiceNow instance and append the following path to the URL:  

