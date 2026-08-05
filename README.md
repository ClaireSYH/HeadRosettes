[README.md](https://github.com/user-attachments/files/30733909/README.md)



# HeadRosettes

## Project Documentation
[View the full project portfolio](docs/HeadRosettes Project Portfolio.pdf)

HeadRosettes is a database-driven e-commerce web application for browsing, comparing, purchasing, and reviewing headphones. The project was developed by a three-member team to apply core web development, database, security, API integration, and data-visualization concepts in a complete service workflow.

## Project Overview

The application supports the full user journey from account registration and product discovery to checkout, order tracking, review submission, and customer inquiries. It also includes administrator tools for content management, delivery-status updates, sales analysis, and PDF export.

**Team size:** 3  
**Role:** Project Lead  
**Application type:** Headphone e-commerce platform  
**Database design:** 15 relational tables

## Key Features

### Product Discovery

- Browse detailed headphone information and customer reviews
- Filter products by:
  - Brand
  - Price
  - Noise-cancellation support
  - Wired or wireless connectivity
- Compare two products by price, weight, noise-cancellation support, and other specifications
- Highlight the generally preferred value in each comparison category
- Display the five best-selling products on the main page based on purchase data

### User Accounts

- Register users with Spring Security
- Validate usernames and passwords using regular expressions
- Check username availability and password confirmation
- Enter postal codes and addresses through the Kakao Address API
- Update profiles using existing database information
- Require password re-entry before account deletion
- Prevent deleted usernames from being reused

### Shopping and Payment

- Add products to the shopping cart
- Adjust product quantities
- Purchase products directly from the product detail page
- Apply reward points partially or in full
- Process payments through the Kakao Pay API
- Display order details after successful payment

### Reviews and Customer Support

- Allow users to write reviews after delivery is completed
- Create reviews with the Summernote editor
- Display the purchased product, publication date, view count, and like count for each review
- Allow users to like reviews and visually identify reviews they have liked
- Show product reviews directly on each product detail page
- Toggle individual reviews and corresponding administrator responses
- Award reward points when an administrator replies to a review
- Submit categorized Q&A posts
- Track inquiry status as `Pending`, `In Review`, or `Resolved`
- Display each user's submitted reviews and Q&A posts

### Community and Store Information

- Provide notice and event boards managed by administrators
- Display offline listening-shop locations through the Kakao Maps API
- Show store details such as address and phone number
- Include a linked YouTube video on the main page

### Administrator Dashboard

- Manage notices, events, orders, inquiries, and delivery status
- Enable review submission only after delivery completion
- Visualize best-selling products and product preferences by gender using Google Charts
- Export dashboard information as a PDF file

## System Structure

The application separates functionality across three primary user roles:

- **Guest:** Browse products, notices, events, store information, and public content
- **Member:** Manage an account, compare products, place orders, use reward points, submit reviews, and create inquiries
- **Administrator:** Manage content, orders, delivery status, customer inquiries, and analytical dashboards

The database consists of 15 tables covering user accounts, products, product options, brands, carts, orders, payments, reviews, likes, notices, events, and Q&A data.

## Technology Stack

### Backend

- Java 8
- Spring Framework
- Spring Security
- JSP
- Maven
- Apache Tomcat 9

### Frontend

- HTML5
- CSS
- JavaScript
- jQuery
- Ajax
- Summernote

### Database

- MySQL
- HeidiSQL

### APIs and Libraries

- Kakao Address API
- Kakao Maps API
- Kakao Pay API
- Google Charts
- iTextPDF
- JSON

### Development Tools

- Spring Tool Suite
- GitHub
- Windows 10

## Main User Flow

```text
Sign Up / Login
        ↓
Browse or Filter Products
        ↓
View Product Details
        ↓
Compare Products or Add to Cart
        ↓
Apply Reward Points
        ↓
Pay with Kakao Pay
        ↓
View Order Confirmation
        ↓
Delivery Completion
        ↓
Write a Review or Submit a Q&A Post
```

## Notable Implementation Details

- Designed a relational database with 15 interconnected tables
- Applied role-based access control for members and administrators
- Integrated multiple external APIs for address search, mapping, and payment
- Connected order status with review eligibility
- Used purchase data to generate product rankings and administrator analytics
- Implemented PDF generation for exporting dashboard information
- Designed product comparison and filtering features to support faster purchase decisions

## Project Screens

The project includes the following major screens:

- Main and About pages
- Sign-up, login, profile update, and account deletion
- Product list, filtering, comparison, and detail pages
- Shopping cart, checkout, and order confirmation
- My Page and purchase history
- Product review board
- Q&A board and personal post history
- Notice and event boards
- Offline listening-shop map
- Administrator dashboard

## Future Improvements

Potential improvements identified after development include:

- Rebuilding the project with a more modern technology stack
- Improving the overall design and user interface
- Expanding the product catalog
- Adding more product images and richer product information

## Demo

A demonstration video was prepared as part of the project portfolio.

> Add the video URL here when available.

## Project Lead

**Sunyoung Hwang**  
Led the three-member project team and contributed to the development and presentation of the application.
