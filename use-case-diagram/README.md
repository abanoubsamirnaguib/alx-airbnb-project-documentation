# Airbnb Clone Backend - Use Case Diagram

This directory contains the use case diagram for the Airbnb Clone Backend system, visualizing the interactions between different actors and the system's key functionalities.

## 📋 Overview

The use case diagram captures all the essential interactions between users (actors) and the Airbnb Clone Backend system. It provides a comprehensive view of system functionality from the user's perspective.

## 🎭 Actors

### Primary Actors

1. **Guest** 
   - Regular users who search for properties and make bookings
   - Can register, browse listings, make reservations, and leave reviews

2. **Host**
   - Property owners who list their properties on the platform
   - Inherit all guest capabilities plus property management features
   - Can create listings, manage bookings, and interact with guests

3. **Admin**
   - System administrators with full system access
   - Responsible for user management, content moderation, and system monitoring

### External Actors

1. **Payment Gateway**
   - External service for processing payments and refunds
   - Integrates with the system for secure financial transactions

2. **Email Service**
   - External service for sending notifications and communications
   - Handles password resets, booking confirmations, and other email communications

## 🎯 Use Cases by Category

### Authentication & User Management
- **Register Account**: User creates a new account on the platform
- **Login**: User authenticates to access the system
- **Manage Profile**: User updates personal information and preferences
- **Reset Password**: User recovers account access via email
- **Enable 2FA**: User adds two-factor authentication for security

### Property Search & Discovery (Guest)
- **Search Properties**: Guest searches for accommodations based on criteria
- **View Property Details**: Guest examines detailed property information
- **View Reviews**: Guest reads reviews from previous guests

### Booking Management (Guest)
- **Make Booking**: Guest reserves a property for specific dates
- **Manage Bookings**: Guest views and manages their reservations
- **Cancel Booking**: Guest cancels a reservation with appropriate policies

### Payment Processing
- **Make Payment**: Secure payment processing for bookings
- **Request Refund**: Guest requests refund for cancelled bookings

### Review System
- **Write Review**: Guest provides feedback after their stay
- **View Reviews**: All users can read property and user reviews

### Property Management (Host)
- **Create Property Listing**: Host adds new property to the platform
- **Manage Property Listings**: Host updates property information
- **Update Availability**: Host manages property calendar and availability
- **Set Pricing**: Host defines pricing structure and policies
- **Manage Host Bookings**: Host handles booking requests and confirmations
- **Respond to Reviews**: Host replies to guest reviews
- **View Host Analytics**: Host accesses performance metrics and insights

### Communication System
- **Send Messages**: Direct messaging between guests and hosts
- **Receive Notifications**: System notifications via email, SMS, or push notifications

### Administrative Functions (Admin)
- **Manage Users**: Admin controls user accounts and access
- **Moderate Content**: Admin reviews and moderates user-generated content
- **Approve Listings**: Admin approves new property listings
- **Monitor System**: Admin oversees system performance and health
- **Generate Reports**: Admin creates analytics and business reports
- **Manage Payments**: Admin handles payment disputes and issues
- **Backup System**: Admin manages data backup and recovery

### Security Features
- **Verify Identity**: System verifies user identity for security
- **Fraud Detection**: Automated fraud prevention and detection

## 🔗 Key Relationships

### Include Relationships
- **Make Booking** includes **Make Payment**: Every booking requires payment processing
- **Register Account** includes **Verify Identity**: Account registration requires identity verification
- **Make Payment** includes **Fraud Detection**: All payments are subject to fraud detection

### Actor Inheritance
- **Host** inherits all capabilities of **Guest**: Hosts can perform all guest activities plus host-specific functions
- **Admin** has unique administrative capabilities but also uses basic authentication features

### External System Integration
- **Payment Gateway** processes all financial transactions
- **Email Service** handles all system communications and notifications

## 📁 Files in this Directory

- `airbnb-use-case-diagram.drawio` - The Draw.io source file containing the complete use case diagram
- `airbnb-use-case-diagram.png` - Exported PNG image of the use case diagram (to be generated)
- `README.md` - This documentation file

## 🎨 Diagram Color Coding

- **Blue (Guest Use Cases)**: Functions available to guest users
- **Green (Host Use Cases)**: Functions specific to host users
- **Yellow (Admin Use Cases)**: Administrative functions
- **Red (Security Use Cases)**: Security-related functions
- **Purple (Communication)**: Communication and notification features
- **Purple (External Actors)**: External system integrations

## 🔧 How to Use

1. Open `airbnb-use-case-diagram.drawio` in Draw.io (app.diagrams.net)
2. The diagram provides a comprehensive view of system functionality
3. Use this diagram for:
   - Requirements analysis
   - System design planning
   - Development task breakdown
   - Testing scenario creation
   - Stakeholder communication

## 📊 Statistics

- **Total Use Cases**: 32
- **Primary Actors**: 3
- **External Actors**: 2
- **Guest-specific Use Cases**: 15
- **Host-specific Use Cases**: 7
- **Admin-specific Use Cases**: 7
- **Security Use Cases**: 2
- **Communication Use Cases**: 2

This use case diagram serves as a foundational document for understanding the complete scope of the Airbnb Clone Backend system and guides the development process by clearly defining user interactions and system boundaries.
