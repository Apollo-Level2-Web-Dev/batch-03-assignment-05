<h1 align="center">4. Bike Rental Service Website</h1>

<h3 align="center">⚠️ Read the entire requirement thoroughly. Every detail must be carefully reviewed from start to finish.</h3>

---
  

You are required to develop a Bike Rental Booking System that incorporates various key features. **The objective of this assignment is to integrate the frontend with the backend system developed in Assignment 3.** This project will test your ability to create a functional, user-friendly web application with a focus on UI/UX design, authentication, and management systems. You'll be implementing components like user authentication, bike management, rental booking, and more. Additionally, you will have the opportunity to enhance the user experience with features like coupon codes, side-by-side bike comparisons, micro-animations, and a dark mode option.

#   

# Detailed Requirements:

## Main Requirements:

### **1.** **Navbar & Footer**

*   A navbar with logo and necessary menu items
*   A meaningful footer. Must contain social media icons and the websites' page links

###   

### **2\. Home Page**

*   **Hero Section:** A prominent banner with a background image or video related to bikes and relevant information.
    *   **Featured Section:** Available bike with brand names, images and View Detail button.
    *   **Testimonials**: Short reviews from satisfied customers.
    *   **Why Choose Us:** List of key benefits or unique selling points (e.g., best prices, wide selection of bikes, excellent customer service).
    *   **Coupons & Discounts Section: \[Bonus\]**
        *   Section highlighting any active promotions or discount codes.
        *   Brief description of how to use the coupons.
    *   **Contact Us Section:** A form with relevant fields.

###   

### **3\. User Authentication:**

**_You must create an admin and must submit the credentials with the other necessary links_**

#### **Sign Up Page:**

\- **Form fields:** Name, Email, Password, Phone, Address

\- **Validation:** Ensure all fields are required are correctly provided

\- **Success:** Redirect to login page with success message

**Note:** By default, every user will have the "USER" role. Initially, there should be an admin in the database. Later, that admin can promote a user to the "ADMIN" role.

  

#### **Login Page:**

\- **Form fields:** Email, Password

\- **Validation:** Ensure all fields are required are correctly provided

\- **Success:** Redirect to the dashboard

###   

#### **Protected Dashboard Routes:**

\- Ensure only authenticated users can access certain routes

\- Implement role-based access (Admin/User)

  

  

### **4\. User Profile Management:**

  

#### **Profile Page:**

\- Display user/admin details

\- Allow user/admin to update their profile information

  

### **4\. Bike Management:**

  

**Bike Listing Page:**

\- Display a list of available bikes with filters for brand, model, availability and a View Detail button redirecting user to the Bike Detail Page.

  

**Bike Detail Page:**

\- Display detailed information about the selected bike (Description, Price, CC, Year, Brand, Availability)

\- If the user is an **Admin**, provide options to edit or delete the bike

\- Implement a "Book Now" button for **users** to start the rental process

  

### **5\. Bike CRUD Operation (Admin Only):**

**Create/Edit Bike Form:**

\- Admins can create or update bike details

\- Form fields: Name, Description, Price, CC, Year, Model, Brand and others

\- Validation: Ensure all fields are required, with appropriate constraints (e.g., year should be a valid year)

**Delete Bike:**

\- Admins can delete bikes from the system

\- Confirmation dialog before deletion

  

### **6\. Rental Management:**

  

**Booking Process:**

**Book Now Button:**

\- Available on the Bike Detail page for users

\- On click, open a modal/form with relevant fields including start time to confirm booking

  

**Rental Confirmation:**

\- Confirm booking details and update bike availability

\- Store booking data and display a success message

  

### **7\. Rentals:**

  

**Return Bike (Admin Only):**

\- Admin can check the list of rental details

\- Calculate button will be available in each rental detail to update the status and calculate the cost by submitting the end time

  

**My Rentals Page:**

It will be Tab system. By default the Unpaid tab will be active.

\- The Paid and Unpaid Tabs will show list of all rentals made by the user with details like bike name, start time, return time, total cost. **Except the Unpaid Tab will have a Pay button.**

\- The Pay button will show the total cost of the ride. The Pay button will redirect the users to the Payment Page.

\- .If the payment is successful the Pay button will be removed and it will appear on the Paid tab.

\- Implement Payment Gateway.

  

### **8\. User Management (Admin Only):**

\- Admin can delete a user or make a user admin

###   

### **9\. Error Handling:**

  

**Error Handling:**

\- Implement a consistent error message display for all API failures using Toast notifications

\- Display validation errors next to form fields

  

**No Data Handling:**

\- Show a friendly message when no bikes or rentals are available

  

**404 Page:**

\- Custom 404 page for unmatched routes

  

### **10\. UI/UX:**

  

**UI/UX Quality:**

**The design of the overall website including dashboard is entirely up to you. Make sure to keep it organized, clean and user-friendly.**

*   **Design Principles:**
    *   Implement a clean, modern design with consistent color schemes and typography.
*   **User Experience:**
    *   Ensure smooth navigation, intuitive controls, and accessibility considerations.
*   **Responsiveness:**
    *   **Cross-Device Compatibility:**
        *   Ensure the website is fully responsive on mobile, tablet, and desktop devices.

  

## Bonus Features

*   **Coupon**
    *   Implement a coupon functionality where the admin can create and manage all coupon codes. These coupons will be available in the coupon section of the homepage, allowing users to apply them for a 10% discount on their rentals.
    *   Include a gamified feature where users can spin a wheel or play a simple game to win a random discount coupon.
*   **Side-by-Side Comparison:**
    *   Allow users to compare multiple bikes side-by-side, highlighting key features like price, engine capacity, and availability.
*   **Micro-Animations:**
    *   Use subtle animations for interactive elements to enhance the user experience.
*   **Dark Mode:**
    *   Toggle between light and dark mode using TailwindCSS