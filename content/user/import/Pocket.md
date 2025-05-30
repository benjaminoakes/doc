---
title: Pocket
weight: 1
---

## Importing from Pocket

Wallabag offers multiple ways to import your saved Pocket articles:

1. **Using the official Pocket API** (recommended if you have access and prefer a server-based method)
2. **Using the CSV Converter Tool** (recommended if you want to avoid API setup or need an alternative--for example, if importing the Pocket ZIP file on a mobile device)

No matter which method you choose, our goal is to make the transition from Pocket to Wallabag as smooth as possible. There are millions of Pocket users looking for a new home, and we want to offer flexible tools to help everyone migrate successfully.

## Option 1: Import via Pocket API

To use the Pocket API method, you need to create an application on their developer site.

- Create a new application [on the developer website](https://getpocket.com/developer/apps/new)
- Fill in the required fields:
  - Application name
  - Description
  - Permissions: **retrieve**
  - Platform: **web**
- Accept the terms and submit your application

Pocket will give you a **Consumer Key** (e.g., `49961-985e4b92fe21fe4c78d682c1`). Enter this key in the `pocket_consumer_key` field in the Wallabag `Config` menu.

Then:

1. Go to `Import` in the Wallabag menu
2. Click `Import contents` under the Pocket section
3. Click `Connect to Pocket and import data`
4. Authorize Wallabag to access your Pocket account
5. Wait while your data is imported (may take time depending on volume)

---

## Option 2: Import via CSV Converter Tool

The easiest alternative is to use the [**Pocket to Wallabag Converter**](https://benjaminoakes.github.io/pocket-to-wallabag/) tool.

This method is especially useful if:

- The new built-in Pocket CSV importer isn't available or doesn't work for your situation
- You’re on shared hosting or can’t update your Wallabag instance to a version that has the new Pocket CSV importer
- You want to skip API setup
- ZIP file management is awkward (e.g. on Android/iOS)

### How to use the converter

1. **Export from Pocket:**
   - Go to Pocket → Settings → Export
   - Request your data export (you’ll receive a ZIP by email)
   - Download the ZIP file

2. **Convert the data:**
   - Visit the [Pocket to Wallabag Converter](https://benjaminoakes.github.io/pocket-to-wallabag/)
   - Upload your Pocket ZIP file
   - Download the generated CSV in Instapaper format

3. **Import into Wallabag:**
   - Go to Import → **Instapaper**
   - Upload the converted CSV file
   - Wallabag will import your articles with folders and tags
