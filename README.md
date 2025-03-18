# Supermarket Management System

## Project Overview
The Supermarket Management System is a comprehensive C++ console application designed to facilitate the day-to-day operations of a supermarket business. It provides different interfaces for administrators, staff, and customers, each with unique functionalities tailored to their roles.

## Features

### User Management
- **Multiple User Types**: Supports three user categories - Administrators, Staff, and Customers
- **Authentication**: Secure login and registration system
- **Account Creation**: First-time setup creates an admin account automatically

### Admin Features
- **User Management**: Create new admin and staff accounts
- **Inventory Control**: Add, view, update, and delete products
- **Order Management**: View all customer orders and update order status
- **Initial Setup**: Option to populate the system with a predefined list of products

### Staff Features
- **Product Management**: Add new products to inventory
- **Inventory Viewing**: Browse the complete product catalog
- **Product Updates**: Modify product prices, quantities, and categories

### Customer Features
- **Product Browsing**: View available products by category or see the entire catalog
- **Shopping Cart**: Add products, view cart contents, and remove items as needed
- **Order Placement**: Check out and convert cart to an order
- **Order History**: View past orders and their current status

### Inventory Management
- **Categorized Products**: Items organized into 11 different categories like Bakery Products, Fruits, Vegetables, etc.
- **Stock Tracking**: Automatic inventory adjustment when orders are placed
- **Detailed Product Information**: Name, price, quantity, and category for each product

### Order Processing
- **Order Tracking**: Orders saved with customer details, items, and total amount
- **Status Updates**: Order status can be changed by admins (Pending, Approved, In Process, Shipped, Delivered, Cancelled)
- **Detailed Invoices**: Generate receipts showing all purchased items and amounts

## Technical Details

### Data Storage
The application uses file-based storage for persistence:
- `users.txt`: Stores user credentials and types
- `products.txt`: Maintains the product inventory
- `orders.txt`: Records all orders in the system
- `{username}_orders.txt`: Stores order history for individual users

### Data Structures
- **Product**: Stores name, price, quantity, and category
- **CartItem**: Represents products added to a shopping cart
- **Order**: Contains customer info, items purchased, total amount, date, and status

### Directory Structure
The system automatically creates a `user_orders` directory to store order files.

## Usage Guide

### Installation
1. Compile the source code using a C++ compiler
2. Run the executable file
3. On first run, you'll be prompted to create an admin account

### Getting Started
Once you've created the initial admin account:

1. **Login**: Use your credentials to access the system
2. **Admin Setup**: As admin, add products or use the "Add Initial Product List" option
3. **Create Staff**: Add staff accounts to help with inventory management
4. **Manage Inventory**: Add, update, or remove products as needed

### Customer Usage
1. **Register**: New customers need to create an account
2. **Browse Products**: View the available products by category
3. **Add to Cart**: Select products and specify quantities
4. **Checkout**: Review the cart and place the order
5. **Track Orders**: View order history and status updates

## Requirements
- C++ compiler with support for C++11 or higher
- Sufficient file system permissions to create and modify files in the application directory

## Future Enhancements
- Database integration for more robust data storage
- Graphical user interface for better usability
- Advanced inventory analytics and reporting
- Online payment system integration
- Barcode scanning capabilities for physical stores

## Creator
This project was created by Veerendra Vishwakarma (The Codex).

## Contributors
This project was developed as a console-based supermarket management solution to demonstrate object-oriented programming principles and file handling in C++.
