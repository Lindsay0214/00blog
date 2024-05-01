---
title: 'Da Nai Wei Wei: Order Beverages Web App'
description: An online platform for ordering beverages.
publishDate: 'Nov 01 2022'
seo:
  image:
    src: '/project-1.jpg'
    alt: Project preview
---

![Project preview](/project-1.png)

**Project Overview:**
An online platform for ordering beverages. allowing consumers to search for nearby stores based on their current location. Users can select their preferred flavors and sizes and order the drinks they desire online, saving them the wait time at the venue. For example, a large milk tea with less sugar and ice is often humorously abbreviated in the youth slang (e.g., "Da'an Forest Park" becomes "Ansen", "Sun Yat-sen Memorial Hall" becomes "Guoguan"). Such colloquial abbreviations like "da nai wei wei" are used to appeal to the younger consumer demographic. This is the frontend source code, developed using the React framework.

## Introduction

1. Develop a user-friendly mobile app that motivates individuals to adopt sustainable practices in their daily lives.
2. Utilize gamification elements to make sustainable living fun and interactive.
3. Provide educational resources and personalized challenges to empower users to make informed eco-conscious decisions.

## Features

Features

1. **Frontend Features**

1. **User (Consumer)**

- Search for nearby beverage shops based on current location.
- Choose size, ice, and sugar levels before adding items to the cart, and complete the purchase using ECPay.
- Modify or delete current products in the cart.
- View current order items and order history.
- Update user information.
- Backend Features

2. **Shop (Vendor)**

- Upload a brand cover photo for the shop.
- Add, modify, and delete product information.
- Administrator (Admin)

3. **Manage all shops**
- Modify and delete shop information.

## Technology Stack

- Frontend: React Hooks for web app development.
- Styles: Tailwind CSS
- Backend: Express for provide frontend api and user authentication.
- Database: Sequelize data storage.
- Plugins: React Query, React Router, Redux Toolkit, @brainhubeu/react-carousel, **Express-session** for session login implement, **bcrypt** for password salty setting, **dotenv** for env variable
- API: Google API（Place & Distance）, Imgur API, ECpay API

