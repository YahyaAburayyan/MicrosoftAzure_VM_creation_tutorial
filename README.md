# Azure VM Bakery Website Deployment Tutorial

This tutorial provides a step-by-step guide for deploying a simple bakery website on a Virtual Machine (VM) in Microsoft Azure. The project was completed as part of the **COMP4381 (Cloud Computing and Data Security)** course at **Birzeit University**.

## Project Overview
- **Scenario**: Create a website to showcase bakery products using Azure cloud services.
- **Technologies Used**: 
  - Azure Virtual Machines (Windows Server 2022 Datacenter)
  - IIS (Internet Information Services) for web hosting
  - HTML for the website frontend

## Steps Summary

### 1. Create a Virtual Machine (VM) in Azure
- **Subscription**: Azure for Students (free tier)
- **Resource Group**: `Yahya_BZU2`
- **VM Configuration**:
  - **OS**: Windows Server 2022 Datacenter
  - **Size**: Basic B1s (low-cost tier)
  - **Credentials**: 
    - Username: `1221971`
    - Password: `1221971@YahyaAburayyan`
  - **Public IP**: `20.217.17.121`

### 2. Connect to the VM
- Used **Remote Desktop Connection (RDP)** with the VM's IP address and credentials.

### 3. Install and Configure IIS
- Installed **Web Server (IIS)** via Server Manager.
- Enabled default features (Static Content, HTTP Errors, etc.).

### 4. Deploy the Website
- **HTML File**: `index.html` (saved in `C:\inetpub\wwwroot\New folder`)
  ```html
  <!DOCTYPE html>
  <html>
  <head>
      <title>BZUBakery</title>
  </head>
  <body>
      <h1>Welcome to BZUBakery!</h1>
      <p>Contact: +972589969</p>
      <ul>
          <li><a href="https://facebook.com/bakery">Facebook</a></li>
          <li><a href="https://twitter.com/bakery">Twitter</a></li>
      </ul>
  </body>
  </html>
