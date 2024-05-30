
# HACXK APK Scraper

![GitHub](https://img.shields.io/github/license/hacxk/hacxkapkscraper)

A Node.js package for scraping APK information from websites.

## Installation

You can install the package via npm:

```bash
npm i hacxkapkscraper
```

## Usage

```javascript
// Import the hacxkAPKScraper function from the 'hacxkapkscraper' package
const { hacxkAPKScraper } = require('hacxkapkscraper');

// Define an asynchronous function to test the hacxkAPKScraper function
async function test() {
    // Specify the URL to scrape
    const url = 'com-zhiliaoapp-musically';
    try {
        // Call the hacxkAPKScraper function with the specified URL
        const result = await hacxkAPKScraper(url);
        // Log the result to the console
        console.log(result);
    } catch (error) {
        // Log any errors to the console
        console.error('Error:', error);
    }
}

// Call the test function
test();
```

Replace `com-zhiliaoapp-musically` with the URL of the APK (e.g., `com-android-vending`).

## API

### `hacxkAPKScraper(url: string): Promise<object>`

This function scrapes APK information from the provided URL and returns a Promise that resolves to an object containing the scraped data.

- `url`: The URL of the APK information page.

**Example Result:**

```json
{
  "author": "HACXK",
  "github": "https://github.com/hacxk",
  "apkInfo": {
    "title": "TikTok",
    "description": "discover, make and share short videos in this social network.",
    "packageName": "com.zhiliaoapp.musically",
    "version": "34.9.1 (2023409010)",
    "fileSize": "378.9 MB",
    "updated": "May 22, 2024",
    "minAndroidVersion": "Android 5.0 (Lollipop, API 21)",
    "screenDPI": "nodpi",
    "architecture": "universal",
    "md5": "601725378a9f3fbee7060c55c37d89e0",
    "sha1": "2897e1b86fe3762f5614b24da4dbbc0d3e1a9c82",
    "downloadLink": "https://r-static-assets.androidapks.com/rdata/xxxxxxxx/com.zhiliaoapp.musically_v34.9.1-2023409010_Android-5.0.apk"
  }
}
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

