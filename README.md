# Reddit Leads Tracker - Make.com Blueprint

This repository contains a **Make.com (formerly Integromat)** blueprint designed to automate the process of finding and tracking Android app testing leads from Reddit.

## 🚀 How it Works

The workflow consists of four main steps:

1.  **RSS Trigger**: Monitors new posts from a curated list of Reddit subreddits related to Android testing:
    *   `r/AndroidClosedTesting`
    *   `r/AndroidAppTesting`
    *   `r/AndroidAppTesters`
    *   `r/AndroidTesting`
    *   `r/playtesters`
    *   `r/TestMyApp`
2.  **Filtering**: Only processes posts that contain specific keywords like "test" or "v2v" (Version to Version) in the title.
3.  **Email Notification**: Sends an automated email via Gmail with the post details (Title, URL, and Description) to the configured recipient.
4.  **Google Sheets Logging**: Automatically logs every relevant lead into a Google Sheet titled `Reddit Leads Tracker` for further management. Data logged includes:
    *   Title
    *   Hyperlink to the post
    *   Author
    *   Date Found

## 🛠️ Setup Instructions

1.  **Download the Blueprint**: Download the `Integration RSS.blueprint.json` file from this repository.
2.  **Import to Make.com**:
    *   Log in to your [Make.com](https://www.make.com/) account.
    *   Create a new scenario.
    *   Click on the three dots (...) at the bottom menu and select **Import Blueprint**.
    *   Upload the `.json` file.
3.  **Configure Connections**:
    *   **Gmail**: Re-authenticate or select your Gmail connection in the "Send an Email" module.
    *   **Google Sheets**: Connect your Google account and select (or create) a spreadsheet named `Reddit Leads Tracker` with columns for Title, Link, Author, and Date.
4.  **Save and Run**: Save the scenario and turn it on to start tracking leads!

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. Free for anyone to use, modify, and distribute.
