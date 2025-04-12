![Pipeline](https://github.com/trantrieuvy/headless-scraper/blob/main/pipeline.png)
# 🖼️ Headless Browser Image Scraper

This project automates the process of scraping high-resolution images from web-based portfolios or gallery websites where full-size images are only accessible after clicking on thumbnails.

## 🔍 How it Works

- **Headless Browser**: Uses Selenium to launch a headless Chrome browser that can render JavaScript-heavy pages — useful for bypassing client-side rendering or CDN restrictions (e.g., Cloudflare).
- **HTML Parsing**: Once the page is fully rendered, BeautifulSoup parses the HTML to extract all project or image links embedded in thumbnail `<a>` tags.
- **Image Extraction**: For each thumbnail/project link, the script opens the full image page and extracts the high-resolution image URLs.
- **Image Downloading**: All collected image URLs are saved and downloaded into a local directory.

## 📁 Features

- Headless and automated scraping for efficient batch downloading.
- Handles JavaScript-rendered pages.
- Filters and stores unique high-resolution image URLs.
- Can be adapted for other image-rich portfolio/gallery websites.

## 🚀 Usage

1. Clone the repository:
   ```bash
   git clone git@github.com:trantrieuvy/headless-scraper.git

2. Instal dependencies:
    ```bash
    pip install selenium beautifulsoup4 requests

3. Run the notebook [scrape_images.ipynb](https://github.com/trantrieuvy/headless-scraper/blob/main/scrape_images.ipynb)
