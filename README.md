## Image-Crawler

A robust, automated image scraping tool that reads keywords from an Excel file and downloads high-quality images from Google Images. This script is optimized with user-agent rotation, download tracking, and retry logic to ensure efficiency and scalability across multiple keyword searches.

📌 Project Overview
This script facilitates the following:

Automatically reads search keywords from an Excel sheet.

Downloads high-resolution images for each keyword from Google Images.

Organizes images into keyword-specific folders.

Avoids duplicate downloads using a local tracking file.

Handles failed requests with retry logic.

Simulates human-like browsing using user-agent rotation.

🛠️ Technologies Used
Python 3.7+

icrawler – For crawling and downloading images.

pandas – For reading Excel input.

openpyxl – Excel engine used by pandas.

logging – For real-time monitoring of crawl progress.

Features
Reads keywords from the first column of keywords.xlsx.

Saves up to 30 images per keyword (customizable).

Downloads only high-resolution images (minimum 500×500).

Maintains a completed.txt file to track previously downloaded images.

Randomly rotates user-agents to avoid detection.

Includes retry logic to ensure reliability across unstable connections.
⚙️ Configuration Options
To customize the crawler:

Change the number of images per keyword:
Edit num_images=30 in the download_images() function call.

Change output directory:
Update the save_dir argument inside download_images().

Modify minimum resolution:
Edit min_size=(500, 500) in the crawl() function.

⚠️ Disclaimer
This project is intended strictly for educational and research purposes.
Please ensure compliance with Google’s Terms of Service and avoid misuse or abuse of web scraping practices.

