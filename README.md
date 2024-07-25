# Deal Buddy

Deal Buddy is a web application built with Next.js that allows users to input the URL of an Amazon product. The app scrapes Amazon to display the current highest, lowest, and average prices of the product. Users can also track the product's price and receive notifications when the price drops.

## Features

- **Product Price Scraping**: Input an Amazon product URL to see the current highest, lowest, and average prices.
- **Price Tracking**: Track the price of a product and receive notifications via email when the price drops.
- **Cron Jobs**: Automated price checking at regular intervals using cron jobs.

## Tech Stack

- **Frontend**: Next.js, Headless UI, Tailwind CSS
- **Web Scraping**: Cheerio, Bright Data
- **Cron Jobs**: Node-cron
- **Notifications**: Nodemailer (for email notifications)
- **Database**: MongoDB

## Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/YourUsername/DealBuddy.git
   cd DealBuddy
