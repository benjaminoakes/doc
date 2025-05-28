---
title: Pocket
weight: 1
---

## Import Methods

There are two ways to import your Pocket data into wallabag:

1. [**CSV Converter Tool**](https://benjaminoakes.github.io/pocket-to-wallabag/) (simple, runs in your browser, no setup required)
2. **Direct API Import** (requires developer setup)

## Method 1: CSV Converter Tool

The easiest way to import your Pocket data is using the [**Pocket to Wallabag Converter**](https://benjaminoakes.github.io/pocket-to-wallabag/) tool.

This method is particularly useful for users who want a simple, straightforward import process and want to avoid API setup complexity.  It achieves this by converting from Pocket format to Instapaper format.

### Features

- **No API setup required** - works with Pocket's standard export
- **100% client-side processing** - your data never leaves your device
- **Open source** - fully auditable code

### How to use the converter

1. **Export from Pocket:**
   - Go to Pocket Settings → Export
   - Wait for the ZIP file to be generated and emailed to you
   - Download your data as a ZIP file

2. **Convert the data:**
   - Visit the [Pocket to Wallabag Converter](https://benjaminoakes.github.io/pocket-to-wallabag/)
   - Choose your Pocket export ZIP file
   - Save the converted, Instapaper-formatted CSV file

3. **Import to Wallabag:**
   - In your Wallabag instance, go to Import → Instapaper
   - Upload the converted CSV file
   - Your articles will be imported with proper folders and tags

## Method 2: Direct API Import

### Create a new application on Pocket

To import your data from Pocket using the API, you need to
create a new application on their developer website to continue.

-   Create a new application [on the developer
    website](https://getpocket.com/developer/apps/new)
-   Fill in the required fields: application name, application
    description, permissions (only **retrieve**), platform (**web**),
    accept the terms of service and submit your new application

Pocket will give you a **Consumer Key** (for example,
49961-985e4b92fe21fe4c78d682c1). You need to configure the
`pocket_consumer_key` in the `Config` menu.

Now, all is fine to migrate from Pocket.

### Import your data into wallabag

Click on `Import` link in the menu, on `Import contents` in Pocket
section and then on `Connect to Pocket and import data`.

You need to authorize wallabag to interact with your Pocket account.
Your data will be imported. Data import can be a demanding process for
your server.
