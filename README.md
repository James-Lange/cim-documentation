# cim-documentation
Splunk dashboard containing documentation for mapping field names to CIM datamodels. 
The ideal use case is to help airgapped Splunk Admins map fields to be CIM compliant. Instead of printing documentation for the CIM field values, this dashboard will provide all documentation for CIM field names and values by datamodel. 

## Screenshot
<img width="2832" height="1593" alt="DashboardPreviewScreenshot" src="https://github.com/user-attachments/assets/d772df26-b231-4b8a-90b9-7fff1990086a" />

## Files
| Name  | Description |
| ------------- |:-------------:|
| cim_lookup_dashboard.xml | Dashboard file for easily navigating documentation. |
| cim_dashboard.csv | Lookup file that contains the field name, description, data model, type, and notes from documentation. |

## Installation Guide (Super Easy)

### Prerequisites
1. Have access to Splunk Web. 
2. Files downloaded from the GitHub repository:
* `cim_lookup_dashboard.xml` (Dashboard)
* `cim_dashboard.csv` (Lookup)

### Step 1: Upload the Lookup File

1. Log in to Splunk Web.
2. Navigate to: `Settings > Lookups > Lookup table files`
3. Click Add new.
4. Select the App where you want the lookup to reside (e.g., search or your custom app).
5. Click Choose File and upload cim_dashboard.csv.
6. Click Save.

> Important: Make sure the lookup file has global permissions and is shared to the appropriate users/admins. 

### Step 2: Install the Dashboard

1. Navigate to:

```Apps > Search & Reporting > Dashboards```

2. Click Create New Dashboard.
Enter:

```
Title: CIM Documentation
Permissions: Set as needed.
```

3. Click Create Dashboard using Dashboard Studio.
In the dashboard editor:
* Switch to Source mode.
* Copy the contents of cim_lookup_dashboard.xml from the GitHub repo.
* Paste into the source editor.

4. Click Save.


## Authors
[James Lange - Principal Engineer](https://www.linkedin.com/in/jamesclangeii/)

[Rishi Ayyagari - Cybersecurity Intern](https://www.linkedin.com/in/rishiayyagari/)
