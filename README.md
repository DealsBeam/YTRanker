# YTRanker - YouTube Backlink Generator for Blogger


## Table of Contents

* [Overview](#overview)
* [🚀 Features](#-Features)
* [🔧 How It Works](#-how-it-works)
* [📌 Requirements](#-requirements)
* [🛠️ Setup Instructions](#-setup-instructions)

  * [Step 1: Get a YouTube Data API Key](#step-1-get-a-youtube-data-api-key)
  * [Step 2: Find Your YouTube Channel ID](#step-2-find-your-youtube-channel-id)
  * [Step 3: Configure Your Blogger Template](#step-3-configure-your-blogger-template)
* [🧠 SEO & Backlinking Strategy](#-seo--backlinking-strategy)
* [📊 Expected Results](#-expected-results)
* [⚠️ Important Notes](#-important-notes)
* [🙏 Acknowledgements](-#acknowledgements)
* [📄 License](#-license)
* [☕ Support This Project](#-support-this-project)

   
## Overview

Introducing YTRanker ,an easier way to grow your YouTube channel.
YTRanker is a free, open-source Blogger template that automatically turns your blog into a YouTube video gallery. It pulls videos directly from your channel, adds them to your site, and creates backlinks to boost your SEO and channel visibility.

Once you set it up, there’s nothing else to do. Every time you upload or delete a video, your blog updates automatically ,no coding, no manual changes.
Just set it and forget it. More views, more engagement, more growth, on autopilot.

## 🚀 Features

- ✅ **Automatic Content**: Fetches latest videos from any YouTube channel
- ✅ **Channel Branding**: Displays channel name, logo, description, and video stats
- ✅ **SEO Optimized**: Adds structured data, Open Graph tags, and canonical links
- ✅ **Performance**: Lazy loads thumbnails for better page speed
- ✅ **User Experience**: Supports infinite scroll & "Load More" button
- ✅ **Engagement**: Includes modal popup to play videos directly on the site
- ✅ **Organization**: Filters videos by tags/categories dynamically
- ✅ **Backlinks**: Auto-generates do-follow backlinks via embedded video links

## 🔧 How It Works

Once you enter your YouTube API key and channel ID in the script:

```javascript
// Configuration
const apiKey = 'YOUR_API_KEY';
const channelId = 'YOUR_CHANNEL_ID_NUMBER';
```

The script performs the following:

1. Fetches channel details including name, logo, subscriber count, and description using the YouTube Data API v3
2. Retrieves recent videos using search and videos API endpoints
3. Processes each video:
   - Formats view counts, durations, and published dates
   - Adds categories based on video tags for filtering
   - Embeds each video using an iframe and links them back to YouTube, creating a backlink
4. Generates SEO Metadata:
   - Dynamic page title, meta description, keywords
   - Open Graph (OG) tags for social sharing
   - JSON-LD structured data for better search engine visibility
5. Displays content in a gallery layout with:
   - Responsive thumbnails
   - Hover effects
   - Clickable modal popup to watch videos

## 📌 Requirements

- Google account
- YouTube Data API v3 key
- Blogger/Blogspot website
- YouTube channel ID

## 🛠️ Setup Instructions

### Step 1: Get a YouTube Data API Key

1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create a new project or select an existing one
   
   1. ![Create New Project](https://github.com/user-attachments/assets/89a5cbe2-e7ec-4b07-90b3-119df471f9f4)
   2. ![Image](https://github.com/user-attachments/assets/3996a1ba-c5ec-4e3c-967c-37eb9a5d6762)
   3. ![Image](https://github.com/user-attachments/assets/01d7408e-4c9d-41ed-9c23-385f6f89f051)
   4. ![Image](https://github.com/user-attachments/assets/8a3e68ef-bf51-49c9-b753-26090f0ae4f4)
   5. ![Image](https://github.com/user-attachments/assets/ebdccd08-3be7-4c1a-abe8-45a1f64809e1)
   6. ![Image](https://github.com/user-attachments/assets/78036bdb-db88-4dd8-8a40-f3ad78fb20c3)


3. Navigate to "APIs & Services" > "Library"
4. Search for "YouTube Data API v3" and click on it
   
   ![YouTube Data API](https://github.com/user-attachments/assets/75173a40-f0e3-4d37-a856-5234a36f062e)

5. Click "Enable"
   
   ![Enable API](https://github.com/user-attachments/assets/99b228c5-750b-4e34-9a33-7e1cdfb7b853)

6. Go to "Credentials" and click "Create Credentials" > "API key"
   
   ![Create Credentials](https://github.com/user-attachments/assets/93e58848-7979-4a46-a5fc-fbc6ff86be48)
   ![Image](https://github.com/user-attachments/assets/5168bad0-ade6-45eb-8cc0-614ce85cca2a)


7. Copy your new API key

### Step 2: Find Your YouTube Channel ID

1. Visit [YouTube](https://www.youtube.com/)
2. Search for the channel you want to embed
3. Go to the channel page
   
   ![Channel Page](https://github.com/user-attachments/assets/3d210e4b-2b99-4ae5-9978-d72ef17b753c)

4. Click on "Share" or "More info" from the channel
5. Click "Share channel" and copy the channel ID
   
   ![Share Channel](https://github.com/user-attachments/assets/8e0fe184-3f8d-4f5b-a692-dc01204be5f4)

### Step 3: Configure Your Blogger Template

1. In your Blogger dashboard, go to "Theme" > "Edit HTML"
2. Search for the configuration section (Ctrl+F and search for "Configuration")
3. Replace the placeholders with your actual API key and channel ID:

```javascript
// Configuration
const apiKey = 'YOUR_API_KEY';    // Replace with your actual API key
const channelId = 'YOUR_CHANNEL_ID_NUMBER';   // Replace with your actual channel ID
```

![Configuration](https://github.com/user-attachments/assets/e2180912-0ca5-4321-81b6-82a90cce51cb)

4. Save your changes

## 🧠 SEO & Backlinking Strategy

By embedding YouTube videos on your Blogspot pages:

- You create backlinks to the original YouTube videos via the iframe src and canonical URLs
- Your blog benefits from fresh dynamic content from your YouTube channel
- The template includes structured data (VideoObject and ItemList), improving your search engine visibility
- Videos increase time-on-site metrics, reducing bounce rates

## 📊 Expected Results


![Results](https://github.com/user-attachments/assets/b7ca0d21-c2c8-4677-9eca-d5790f83f52c)
![Responsive - smart phone](https://github.com/user-attachments/assets/32ef6ecc-73c0-43ea-8f78-e7d1a9e86935)


- Improved YouTube video rankings
- Increased channel visibility
- Better website engagement metrics
- More organic traffic to both your website and YouTube channel

## ⚠️ Important Notes

- The free YouTube Data API has usage quotas. Monitor your usage to avoid exceeding limits.
- Make sure your content complies with both YouTube and Blogger terms of service.
- Keep your API key secure and avoid exposing it in public repositories.

## 🙏 Acknowledgements

Created by saheermk

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

If you find this project helpful, please consider giving it a star ⭐ on GitHub!

---

## ☕ Support This Project

[**Buy Me a Coffee**](https://buymeacoffee.com/saheermk)

<a href="https://buymeacoffee.com/saheermk/"><img src="https://github.com/user-attachments/assets/c22c58cc-8ae2-4c35-bc41-4c6e8ffe99fc" alt="Buy Me a Coffee QR" width="150"/></a>

