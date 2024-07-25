# Deal Buddy

Deal Buddy is a web application built with Next.js that allows users to input the URL of an Amazon product. The app scrapes Amazon to show the current highest, lowest, and average prices of the product. Additionally, users can opt to track the product's price, and the app will notify them when the price drops.

## Features

- **Product Price Scraping**: Input an Amazon product URL to see the current highest, lowest, and average prices.
- **Price Tracking**: Track the price of a product and receive notifications when the price drops.
- **Cron Jobs**: Automated price checking at regular intervals using cron jobs.

## Tech Stack

- **Frontend**: Next.js, Headless UI, Tailwind CSS
- **Web Scraping**: Cheerio, Bright Data
- **Cron Jobs**: Node-cron
- **Notifications**: Nodemailer (for email notifications)
- **Database**: MongoDB

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/DarrenChahal/DealBuddy.git
    cd DealBuddy
    ```

2. Install dependencies:

    ```bash
    npm install
    ```

3. Set up environment variables: Create a `.env` file in the root directory and add the following variables:

    ```plaintext
    # Scraper
    BRIGHT_DATA_USERNAME=
    BRIGHT_DATA_PASSWORD=

    # Database
    MONGODB_URI=

    # Email
    EMAIL_PASSWORD=
    ```

4. Run the development server:

    ```bash
    npm run dev
    ```

5. Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Usage

1. **Enter the Amazon Product URL**: On the home page, paste the URL of the Amazon product you want to track.

2. **View Price Information**: After submitting the URL, you will see the current highest, lowest, and average prices of the product.

3. **Track the Product**: Click on the "Track" button to start tracking the product's price. You will be notified via email when the price drops.
