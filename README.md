# Food Scraper Frontend

React frontend for the Food Image Scraper tool — a production application that automates food image retrieval for restaurant menus. Deployed on Netlify and connected to a Node.js backend running on AWS EC2.

## Live Demo

Frontend hosted on Netlify | Backend API: menu-image-scraper.duckdns.org

## Tech Stack

- **Framework:** React
- **Hosting:** Netlify (CD from GitHub)
- **API:** Connects to Express backend on AWS EC2

## Features

- Clean UI to input restaurant URLs and retrieve food images
- Displays deduplicated image results from the scraper API
- Handles backend proxy responses for hotlink-protected images

## Backend

The backend API for this project: [food-scraper-backend](https://github.com/Vinay-2014/food-scraper-backend)

Deployed on AWS EC2 with Nginx, PM2, and SSL — see backend repo for full architecture details.

## Getting Started

bash
git clone https://github.com/Vinay-2014/food-scraper-frontend
cd food-scraper-frontend
npm install
npm start

Set the backend API URL in your `.env`:

REACT_APP_API_URL=https://menu-image-scraper.duckdns.org
