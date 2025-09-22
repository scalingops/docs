# Syncro Integration Setup Guide

## Overview
This guide will walk you through the process of configuring the Syncro integration with MSPortal. The integration requires an API key from your Syncro account with specific permissions.

## Prerequisites
- Active Syncro account with administrative access
- MSPortal account with integration permissions

## Configuration Steps

### Step 1: Access MSPortal Integration Settings
Navigate to [https://msportal.ai/settings/integrations](https://msportal.ai/settings/integrations) and click the gear icon next to the Syncro integration.

![](https://colony-recorder.s3.amazonaws.com/files/2025-09-19/58747858-5f04-43b9-b089-b3c43493b9bb/stack_animation.webp)

### Step 2: Open Syncro Administration Portal
Log into your Syncro account and access the administration portal.

![](https://colony-recorder.s3.amazonaws.com/files/2025-09-19/400e0b26-00dd-40b0-ae93-773209c67eb9/stack_animation.webp)

### Step 3: Navigate to API Tokens
Scroll to the bottom of the administration portal to locate the API Tokens section.

![](https://ajeuwbhvhr.cloudimg.io/https://colony-recorder.s3.amazonaws.com/files/2025-09-19/c71de32a-d02e-4e4e-8d2d-ab8da9050ace/ascreenshot.jpeg?tl_px=0,227&br_px=1719,1189&force_format=jpeg&q=100&width=1120.0&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=102,437)

### Step 4: Create New API Token
Click the "New Token" button to begin creating your API token.

![](https://ajeuwbhvhr.cloudimg.io/https://colony-recorder.s3.amazonaws.com/files/2025-09-19/ff07341b-183f-445f-9f8b-7288a063cec3/ascreenshot.jpeg?tl_px=187,0&br_px=1906,961&force_format=jpeg&q=100&width=1120.0&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=938,101)

### Step 5: Select Custom Permissions
Choose "Custom Permissions" to configure specific access rights for the integration.

![](https://ajeuwbhvhr.cloudimg.io/https://colony-recorder.s3.amazonaws.com/files/2025-09-19/321f7b41-dfe9-4f7f-bddc-e447b979df4f/ascreenshot.jpeg?tl_px=0,0&br_px=1719,961&force_format=jpeg&q=100&width=1120.0&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=254,247)

### Step 6: Configure Token Settings
1. **Name**: Enter a descriptive name for your token (e.g., "MSPortal Integration")
2. **Expiration**: Set the expiration date to at least one year in the future
3. **Permissions**: Select all permissions from the list below

**Important**: Save your API token immediately after creation. You cannot retrieve it again once you leave this page.

## Required Permissions

Select the following permissions for the API token:

### Asset Management
- Assets - View Details
- Assets - List/Search
- Assets - Edit
- Assets - Create

### Customer Management
- Customers - List/Search
- Customers - View Detail
- Customers - View Total Invoiced
- Contacts - Import

### Tickets & Support
- Tickets - List/Search
- Tickets - View Details
- Tickets - View 'Their Ticket' Details (assigned to them)
- Tickets - Create
- Tickets - Edit
- Tickets - Use Ticket Charges
- Ticket Comments - New
- Ticket Canned Responses - Manage
- Ticket Custom Fields - Manage
- Ticket SLA - Edit
- Ticket Worksheets - Manage
- Ticket Timers - Overview

### Financial
- Invoices - List/Search
- Invoices - View Details
- Estimates - List/Search
- Estimates - View Details
- Estimates - Create
- Estimates - Edit
- Payments - View List
- Recurring Invoices - List

### Other Operations
- Appointments - View All (see-own never restricted)
- Contracts - List/Search
- Products - List/Search
- Pending Orders - View All
- Vendors - List
- Warranties - List
- Warranties - View Details
- Documentation - Allow Usage
- Timelogs - Manage
- RMM Alerts - List

## Step 7: Complete Integration Setup

### Add Token to MSPortal
1. Copy the generated API token from Syncro
2. Return to MSPortal integration settings
3. Paste the token into the API key field
4. Enter your Syncro domain name
5. Click "Save" to activate the integration

![](https://colony-recorder.s3.amazonaws.com/files/2025-09-19/76c9550b-d460-4f68-aca1-cca0783bbd92/stack_animation.webp)

## Synchronization Process

### Initial Sync
- Customer data will begin synchronizing within approximately 1 minute
- Tickets and users will sync alongside customer data
- Devices and additional settings will sync after customers have been imported

### Manual Sync
To force an immediate synchronization of specific data types, use the refresh button in the integration settings.

![](https://ajeuwbhvhr.cloudimg.io/https://colony-recorder.s3.amazonaws.com/files/2025-09-19/981ea464-c9ac-452b-ae90-f2d3c52397c4/ascreenshot.jpeg?tl_px=530,72&br_px=1907,841&force_format=jpeg&q=100&width=1120.0&wat=1&wat_opacity=0.7&wat_gravity=northwest&wat_url=https://colony-recorder.s3.us-west-1.amazonaws.com/images/watermarks/FB923C_standard.png&wat_pad=735,277)

## Important Notes

- **Token Security**: Store your API token securely. If compromised, immediately revoke it in Syncro and generate a new one
- **Sync Timing**: Initial synchronization may take several minutes depending on data volume
- **Dependencies**: Devices and certain settings require customer data to be imported first

## Troubleshooting

If synchronization issues occur:
1. Verify all required permissions are enabled
2. Check the API token hasn't expired
3. Ensure your Syncro domain is correctly entered
4. Use the refresh button to trigger manual synchronization
5. Contact support if issues persist


