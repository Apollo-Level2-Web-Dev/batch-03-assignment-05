<h1 align="center">1. Car Wash Booking System</h1>

<h3 align="center">⚠️ Read the entire requirement thoroughly. Every detail must be carefully reviewed from start to finish.</h3>

---

The Car Wash Booking System frontend is a user-friendly web application designed to simplify the car wash booking process. It features a Home Page with easy navigation, a hero section, and a quick booking call-to-action. Users can sign up or log in securely, browse and filter services, view detailed service information, and book time slots directly through the Service Details pages. The Admin Dashboard allows administrators to manage services, slots, and users. The User Dashboard provides personalized booking history, and the Contact Page enables direct communication.

  

# Detailed Requirements:

## Main Requirements:

### 1\. Home Page

**Features:**

*   **Navigation Menu:** Links to key pages like Services, Booking, Login, and other essential sections.
*   **Hero/Branding Section:** An introductory section with a strong branding message and visuals to communicate the essence of the car wash service.
*   **Call-to-Action Button:** A prominent button encouraging users to book a service, redirecting them to the Services page.
*   **Featured Services:** Display up to six services with brief descriptions and images to highlight the most popular offerings.
*   **Review Section:**
    *   **Input Field & Rating Component:**
        *   A text area for users to leave feedback on their experience with the site.
        *   A star-based rating system (1-5 stars) for users to rate their overall experience.
    *   **Design:** The review section should be visually appealing, using engaging colors, icons, and animations to encourage users to leave feedback. Drawing inspiration from platforms like Dribbble or Pinterest can help create an attractive and interactive design.
    *   **Post-Submission Display:**
        *   After submitting a rating and feedback, the overall site's rating (an average of all submitted ratings) will be displayed.
        *   The last two user reviews, including their respective ratings and comments, will be shown immediately beneath the input field.
        *   **"See All Reviews" Button:** A button that redirects to a dedicated "Reviews" page, where all reviews are displayed in full detail.
*   **Footer:** Contains links to all relevant pages, contact information, and social media links.

---

### 2\. User Authentication Pages

**a) Sign Up Page:**

**Features:**

*   Form fields for name, email, password, phone number, address.
*   By default, every user will have the "USER" role. Initially, there should be an admin in the database. Later, that admin can promote a user to the "ADMIN" role.

**Functionality:**

*   Allows users to create a new account.
*   Form validation (e.g., correct email format).
*   Displays success or error messages based on the outcome.



**b) Login Page:**

**Features:**

*   Form fields for email and password.

**Functionality:**

*   Users can log in to their accounts.
*   Token-based authentication to maintain user sessions.
*   Displays error messages for incorrect credentials or any error.

---

### 3\. Services Page

**Features:**

*   A list of all available car wash services with brief descriptions, prices, and durations.
*   Option for users to view details of each service.

**Functionality:**

*   Allows searching filtering and sorting of services (e.g., by price, duration).

---

### 4\. Service Details Page

**Features:**

*   Detailed information about the selected service.
*   Display available time slots for the selected service on the current date by default.
*   Booked time slots should be disabled and unclickable.
*   Available time slots should be clickable for selection.
*   Optional: A calendar to choose a date, with available slots appearing based on the selected date.
*   A "Book This Service" button appears after selecting a slot.

**Functionality:**

*   Clicking "Book This Service" redirects the user to the Booking page.

---

### 5\. Booking Page

**Features:**

*   **Left Side:** Display of the selected service and time slot. Try to make the design attractive.
*   **Right Side:** A form for submitting user information (User name, email, selected time - auto-filled).
*   A "Pay Now" button for payment processing.

**Functionality:**

*   Upon clicking the "Pay Now" button, the user will be redirected to SSLCOMMERZ/AAMARPAY, and the slot status associated with the booking will be marked as "booked."
*   Redirects the user to a success page after payment.

---

### **6\. Service Slot Countdown**:

After a user creates a booking, display a countdown timer that shows the time remaining until their selected slot. If multiple slots are selected, only the countdown for the immediate next slot will be shown in the navbar. Additionally, in the user's booking history under "Upcoming Bookings," a countdown for each booking will be displayed in the booking card.

---

### 7\. Admin Dashboard

**Features:**

*   Overview of recent bookings (just showing the booking list), user management, Slot management and service management.

**Functionality:**

*   Accessible only to admin users.
*   In the admin dashboard, the service data should be displayed in a tabular format.
*   When implementing the "Add Service" feature, a single "Add Service" button should be provided on the page. Upon clicking this button, a modal containing the service creation form will open. After the user completes and submits the form, the modal will close automatically, and the newly created service will be optimistically updated in the system, providing a real-time experience that enhances the overall user interaction.
*   In each row of the service data table, there should be action buttons for updating and deleting the service data.
*   Upon clicking the update button, the system should either open a modal or redirect the user to a new page, depending on the size and complexity of the data. The fields within the form should be pre-populated with the selected service data, allowing for a smooth and efficient editing process.
*   Before deleting a service, there should be a confirmation pop-up to ensure that the user intends to proceed with the deletion.
*   Ability to create and manage slots for services.
*   An admin should be able to update the slot status individually.
*   An admin should not be able to update the status of a booked slot
*   The admin is authorized to toggle the slot status between AVAILABLE and CANCELLED.
*   View user bookings in a tabular form.
*   User management: view user list, edit user roles.

---

### 8\. User Dashboard

**Features:**

*   Overview of the user’s bookings and account information.
*   View booking history with details of past and upcoming bookings.

**Functionality:**

*   Users should be able to update their profiles, enabling them to manage their personal information.
*   The history of past bookings should be displayed in a tabular format.
*   Upcoming bookings should be displayed in a card format, with a countdown timer positioned in the corner of each card.

---

### 9\. Testimonial Page

**Features:**

*   A form to submit a testimonial, with a restriction allowing each user to submit only one testimonial.
*   Display of testimonials submitted by other users.

**Functionality:**

*   Users are allowed to submit only one testimonial each.
*   Submitted testimonials are displayed on the page for other users to view.

---

### 10\. Error Pages

**Features:**

*   Custom 404 page for when a user navigates to a non-existent route.

**Functionality:**

*   Navigation options to guide users back to a safe page (e.g., Home, Login).

  

* * *

  

### Bonus Requirements

1. **Service Comparison Feature**: Enable users to select and compare two or more services side by side. This feature should clearly display the services’ features, prices, and durations, helping users make informed decisions.
2. **Scroll to Top Button**: Implement a "Scroll to Top" button that appears when users scroll down the page. This button should be easily accessible, allowing users to quickly return to the top of the page with a single click, enhancing navigation and user experience.
3. **UI/UX Improvements**: Focus on enhancing the user interface and experience by implementing design best practices, ensuring the application is intuitive, responsive, and visually appealing.
4. Responsive hote hobe.
5. **GitHub Contributions**: Maintain a well-documented GitHub repository with a minimum of 15 commits. Each commit should represent meaningful progress, such as feature implementation, bug fixes, or UI enhancements.

  

### Deliverables:

*   Fully functional frontend application connected to the backend system.
*   Implementation of all the pages listed above with responsive design.
*   User and Admin dashboards with the features described.
*   Complete integration of the booking system with the backend.
*   The frontend must interact seamlessly with the backend.
*   The UI/UX design should be user-friendly, intuitive, and responsive.
*   Code should be clean, well-organized, and documented.
*   Creative and effective solutions to any challenges faced during the integration process.

###   

**\[ N.B: If you need to add or update anything in the backend of Assignment-3 to meet the above requirements, feel free to do so. \]**