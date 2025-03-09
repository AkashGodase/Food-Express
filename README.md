## Overview
The **Online Food Ordering System** is a web-based application built using **Spring Boot** that enables users to browse restaurants, order food, and manage their accounts. The system also includes an **admin dashboard** for managing restaurants, food items, and orders.

## Features
### User Features
- **User Registration & Authentication** (JWT-based login system)
- **Browse Restaurants and Food Items**
- **Add Items to Cart and Place Orders**
- **View Order History and Track Orders**

### Admin Features
- **Manage Food Items** (`AdminFoodController.java`)
- **Manage Orders** (`AdminOrderController.java`)
- **Manage Restaurants** (`AdminRestaurantController.java`)

### Security & Configuration
- **JWT-based Authentication & Authorization** (`JwtProvider.java`, `JwtTokenValidator.java`)
- **Centralized Application Configuration** (`AppConfig.java`)
- **CORS and Web Configuration** (`WebConfig.java`)

## Technologies Used
- **Backend**: Java, Spring Boot, Spring Security, JWT
- **Database**: MySQL (or other relational databases)
- **Build Tool**: Maven
- **Authentication**: JWT Token-based Authentication

## Setup Instructions
1. **Clone the Repository:**
   ```sh
   git clone <repository-url>
   cd online-Food-Odering
   ```
2. **Configure Database:**
   - Update `application.properties` with your database credentials.
3. **Run the Application:**
   ```sh
   mvn spring-boot:run
   ```
4. **Access the Application:**
   - API Endpoints are available at `http://localhost:8080`
   - Admin panel and user functionalities can be accessed accordingly.

## API Endpoints (Examples)
- **User Login:** `POST /auth/login`
- **Get All Restaurants:** `GET /restaurants`
- **Place an Order:** `POST /orders`
- **Admin - Add Food Item:** `POST /admin/food`

## Future Enhancements
- Integration with Payment Gateways
- Real-time Order Tracking
- Improved UI/UX for users and admins

