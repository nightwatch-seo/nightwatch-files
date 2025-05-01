
# Browser extension dynamic banner instructions

# How to Add New Banners to the Browser Extension

Follow these steps to add new banners to the Nightwatch browser extension:

***

## 1. Visit the Repository

Go to the following GitHub repository:\
👉 https://github.com/nightwatch-seo/nightwatch-files

***

## 2. Upload New Media Files

* Upload the new media files you'd like to include in the banner.
* Ideally, create a new folder to keep your files organized.
* You can drag-and-drop files via GitHub's UI or use Git commands.

***

## 3. Edit `banner-settings.json`

1. Locate and click on the `banner-settings.json` file in the repo.
2. Click the **pencil icon** (edit) in the top right corner to edit the file.
3. Scroll to the list of configured media objects.

***

## 4. Add a New Media Object

At the end of the list (but before the closing bracket if it's an array), add a new object in the following format:

```json
,
{
  "target_url": "https://nightwatch.io/xxxx",
  "media_url": "https://raw.githubusercontent.com/nightwatch-seo/nightwatch-files/main/banner-v5.png",
  "media_type": "image"
}
```

* `target_url`: URL where users should be redirected when clicking the banner.

* `media_url`: Direct GitHub link to your uploaded image/video/gif (hosted via `raw.githubusercontent.com`).\
  To get this link in raw format:

  ```
  1. Click on the media file you added in the GitHub repository.
  1. Click the **"Download"** or **"Raw"** button (usually located near the top right).
  1. Copy the URL from your browser's address bar — it should start with `https://raw.githubusercontent.com/...`
  ```

* `media_type`: Type of media. Acceptable values: `image`, `video`, or `gif`.

***

## 5. Save and Commit

* Scroll down and add a short commit message (e.g., "Add new banner v5").
* Commit the changes directly to the `main` branch or create a pull request, depending on your workflow.

***

## 6. Wait for GitHub Processing

GitHub may take up to **5 minutes** to process and serve the raw media files.

After that, your new banner should be available and visible in the browser extension.

          
