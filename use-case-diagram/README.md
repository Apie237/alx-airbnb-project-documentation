# Use Case Diagram - Airbnb Clone Backend

## Overview
This use case diagram illustrates the key interactions between different actors (users) and the Airbnb Clone backend system. It visualizes the main functionalities and how different user roles interact with the system.

## Actors

### 1. Guest (Unregistered User)
- **Primary Role**: Potential customers who can browse and search properties
- **Capabilities**: Limited access to public information

### 2. Registered User
- **Primary Role**: Authenticated users who can book properties and manage their accounts
- **Capabilities**: Full access to booking and profile management features

### 3. Host
- **Primary Role**: Property owners who list and manage their properties
- **Capabilities**: Property management, booking oversight, and revenue tracking

### 4. Admin
- **Primary Role**: System administrators who manage the platform
- **Capabilities**: Full system access, user management, and content moderation

### 5. Payment Gateway
- **Primary Role**: External system for processing payments
- **Capabilities**: Payment processing, refunds, and transaction management

## Primary Use Cases

### Guest Use Cases
1. **Browse Properties**: View available properties without authentication
2. **Search Properties**: Filter and search for specific properties
3. **View Property Details**: Access detailed property information
4. **Register Account**: Create a new user account
5. **Login**: Authenticate to access additional features

### Registered User Use Cases
1. **Manage Profile**: Update personal information and preferences
2. **Book Property**: Make reservation requests
3. **View Bookings**: Access booking history and current reservations
4. **Cancel Booking**: Cancel existing reservations
5. **Make Payment**: Process payments for bookings
6. **Leave Review**: Rate and review properties and hosts
7. **Send Messages**: Communicate with hosts
8. **Save Properties**: Add properties to wishlist/favorites

### Host Use Cases
1. **List Property**: Create new property listings
2. **Manage Properties**: Update property information and availability
3. **Upload Images**: Add and manage property photos
4. **Set Pricing**: Define pricing and availability calendar
5. **Manage Bookings**: Accept, decline, or modify booking requests
6. **Receive Payments**: Get payouts from successful bookings
7. **Respond to Reviews**: Reply to guest reviews
8. **Communicate with Guests**: Message potential and confirmed guests

### Admin Use Cases
1. **Manage Users**: Oversee user accounts and permissions
2. **Moderate Properties**: Approve and monitor property listings
3. **Handle Disputes**: Resolve conflicts between hosts and guests
4. **Monitor Payments**: Oversee financial transactions
5. **Generate Reports**: Create system analytics and performance reports
6. **Manage Content**: Moderate reviews and user-generated content
7. **System Configuration**: Update system settings and parameters

## Secondary Use Cases

### System Integration Use Cases
1. **Process Payment**: Integration with payment gateway for transactions
2. **Send Notifications**: Automated email and in-app notifications
3. **Validate Data**: Server-side validation of all inputs
4. **Log Activities**: Track system activities for security and analytics
5. **Backup Data**: Regular system data backup operations

### Security Use Cases
1. **Authenticate User**: Verify user identity and credentials
2. **Authorize Actions**: Control access to specific system features
3. **Encrypt Data**: Secure sensitive information transmission
4. **Rate Limit**: Prevent system abuse through API rate limiting

## Use Case Relationships

### Includes Relationships
- **Book Property** includes **Authenticate User**
- **Make Payment** includes **Validate Payment Method**
- **List Property** includes **Upload Images*