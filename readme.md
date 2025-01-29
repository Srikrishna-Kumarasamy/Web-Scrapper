# Web Crawler

## Introduction
This project implements a web crawler that efficiently traverses and extracts web pages using a **Breadth-First Search (BFS)** strategy. The crawler prioritizes new domains before revisiting previously crawled domains, ensuring optimal discovery of content. It is specifically designed to process and analyze web pages within the **New Zealand domain**.

## Features
- **Seed-Based Crawling:** Begins with 20 seed URLs.
- **Priority Queue Management:** Prioritizes new domains before revisiting existing ones.
- **Breadth-First Search (BFS) Strategy:** Ensures level-wise URL traversal.
- **Robots.txt Compliance:** Respects website crawling policies.
- **Duplicate Handling:** Maintains sets for visited URLs and domains to optimize efficiency.
- **Content-Type Validation:** Processes only `text/html` pages.
- **Logging Mechanism:** Stores crawling results, including URL status, page size, and domain details.

## Workflow
1. **Initialize** the crawler with a list of 20 seed URLs.
2. **Process URLs** using a **priority queue** based on depth and domain priority.
3. **Validate URLs** for correctness and check content type.
4. **Check robots.txt** to ensure compliance with the website’s rules.
5. **Fetch content** using `urllib` and extract relevant metadata.
6. **Store results** in a log file for further analysis.
7. **Avoid duplicates** by maintaining sets for seen URLs and domains.

## Requirements
- Python 3.x
- `urllib` for handling web requests
- A working internet connection

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/web-crawler.git
   cd web-crawler
