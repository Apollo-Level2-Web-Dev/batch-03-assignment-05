# #3 Car Rental Reservation System

* * *

### **Frontend Requirements for Car Rental Reservation System**

* * *

#### **Overview:**

The Car Rental System is designed to provide users with a seamless experience when renting cars online. It caters to both customers(users) and administrators(admins). Customers can browse available cars, make reservations, and see their bookings. Administrators, on the other hand, can manage the car inventory, monitor reservations, and maintain the overall system.

  

#### **1\. Home Page**

*   **Header:**
    *   Logo and company name.
    *   Navigation menu: Home, About Us, Booking, Contact.
    *   Login/Sign Up buttons.
*   **Hero Section:**
    *   A large banner image showcasing cars with a prominent "Book Now" call-to-action button.
    *   A search bar for quickly checking car availability based on location and dates.
*   **Featured Cars:**
    *   A carousel or grid display of featured cars with images, brief descriptions, and pricing.
*   **Why Choose Us?**
    *   Highlight unique selling points such as best prices, wide selection, and 24/7 support.
*   **Customer Testimonials:**
    *   A section featuring reviews and ratings from satisfied customers.
*   **Footer:**
    *   Links to social media profiles, privacy policy, terms of service, and contact information.

* * *

#### **2\. User Authentication Pages**

*   **Sign Up Page:**
    *   **Main Form:**
        *   Fields: Name, Email Address, Password, Confirm Password, Phone Number (optional).
        *   Terms & Conditions checkbox with a link to the document. (you may read the document using the link and use the checkbox for the consent).
    *   **Buttons:**
        *   Sign Up button.
        *   Sign In Instead link for existing users.
    *   **Footer:**
        *   Links to Privacy Policy and Terms of Service.
    *   **Validation & Error Handling:**
        *   Real-time validation for email format and matching passwords.
        *   Clear error messages for invalid inputs or if the email is already registered.
        *   Redirect to the login page after successful registration.
*   **Sign In Page:**
    *   **Main Form:**
        *   Fields: Email Address, Password.
    *   **Buttons:**
        *   Sign In button.
        *   Forgot Password? link to a password recovery page.
        *   Sign Up Instead link for new users.
    *   **Footer:**
        *   Links to Privacy Policy and Terms of Service.
    *   **Validation & Error Handling:**
        *   Real-time email validation.
        *   Error messages for incorrect email or password, with a link to recover the password.
        *   Redirect to the dashboard after successful login.

* * *

#### **3\. Admin Dashboard (Manage Cars) \[Private/Protected Route\]**

*   **Dashboard Overview:**
    *   A summary view showing key statistics like total bookings, available cars, revenue, etc.
*   **Manage Cars:**
    *   Add, update, or delete car listings with fields for car details (make, model, year, features, pricing).
    *   Image upload functionality for car photos.
*   **Manage Bookings:**
    *   View and manage customer bookings.
    *   Options to approve, or cancel bookings.
*   **Manage Return Cars:**
    *   **View and Manage Booked Cars:** Access and manage all cars that have been booked.
    *   **Return Options:** Provide the option to return a car. When a car is returned, its status will be updated accordingly, reflecting the car's availability and the completion of the booking process.
*   **User Management:**
    *   Manage customer and admin accounts.
    *   Add, edit, or remove users with different roles (admin).
*   **Reports:**
    *   Generate and view reports on car usage, revenue, and other key metrics. Add printing functionality

* * *

#### **4\. User Dashboard (Manage User Data) \[Private/Protected Route\]**

*   **Overview:**
    *   View personal information and booking history.
    *   Update profile details, such as contact information and preferences.
*   **Booking Management:**
    *   View upcoming and past bookings.
    *   Options to modify or cancel existing bookings.
*   **Payment Management:**
    *   After returning the car a user will be able to pay the amount
    *   Functionality to pay the amount.

* * *

#### **5\. Car Listing Page**

*   Display all available cars in a grid or list view.
*   Filters for car type (e.g., SUV, hybrid, sedan), price range, and other features.
*   Each car entry includes a brief description, image, pricing, and a "View Details" button.

* * *

#### **6\. Car Details Page**

*   Detailed information about the selected car, including features, pricing, availability, and customer reviews.
*   High-quality images with zoom functionality.
*   Options to choose additional features like insurance, GPS, child seat, etc.
*   A prominent "Book Now" button leads to the booking page.

* * *

#### **7\. Booking Page \[Private/Protected Route\]**

*   **Search Form:**
    *   Fields for location, pick-up and drop-off dates, car type, etc.
*   **Search Results:**
    *   A list of available cars based on the search criteria, each with a brief description, image, pricing, and "Book Now" button.
*   **Car Details Modal:**
    *   When a car is selected, a modal window pops up with detailed information about the car, including features, insurance options, and cancellation policy.
*   **Booking Form:**
    *   Enter personal details, payment information, and any additional options (e.g., GPS, child seat).
*   **Booking Confirmation:**
    *   A confirmation page with booking details, a reference number, and an option to print or email the booking.

* * *

#### **8\. About Us Page**

*   **Header:**
    *   Consistent with the Home Page for a cohesive design.
*   **Company History:**
    *   Details about the company’s founding year, mission, and vision.
*   **Our Team:**
    *   Profiles of key team members with photos, names, and roles.
*   **Our Fleet:**
    *   Information about the variety of cars available (economy, luxury, SUVs, etc.).
*   **Values & Commitment:**
    *   Explanation of the company’s commitment to customer service, sustainability, etc.
*   **Contact Information:**
    *   A dedicated section for contact details, including phone number, email, and physical address.

* * *

### 9\. Error Page:

*   Create a visually appealing 404 page that aligns with the overall theme of the site. This page should appear when the user navigates to a route that doesn't exist.
*   In case of an error from the backend API (e.g., "There is no car available right now." or any other message returned when no data is available), display the error message to the user.
*   Ensure that the page includes navigation options to help users find their way back to safe pages, such as Home and Login.

* * *

#### **10\. Responsive Design & UI/UX Requirements**

*   Ensure all pages are fully responsive and provide a seamless experience across devices (mobile, tablet, desktop).
*   Implement intuitive and user-friendly navigation.
*   Use consistent branding elements (colors, fonts, logo) throughout the site.

* * *

#### **Bonus Feature**

*   **Payment System:**
    *   A user can pay the amount after returning the car.
    *   Integrate a secure payment gateway for processing online payments.
    *   Support for multiple payment methods (AmarPay/SSLCommerz any of these local payment methods).
    *   Display a summary of charges before confirming the payment.
    *   A confirmation page with a payment receipt.
*   Theme switcher:
    *   Dark/light/system theme switch.

* * *

**\[ N.B: If you need any modification in the backend of Assignment-3 to meet the above requirements, feel free to do so. \]**