<h1 align="center">1. Car Wash Booking System</h1>

<h3 align="center">⚠️ Read the entire requirement thoroughly. Every detail must be carefully reviewed from start to finish.</h3>

---

**Objective:**

The Car Wash Booking System frontend is a user-friendly web application designed to simplify the car wash booking process. It features a Home Page with easy navigation, a hero section, and a quick booking call-to-action. Users can sign up or log in securely, browse and filter services, view detailed service information, and book time slots directly through the Service Details pages. The Admin Dashboard allows administrators to manage services, slots, and users. The User Dashboard provides personalized booking history.

---

### Public Pages

**1. Home Page**

- **Navigation Menu:** Links to key pages like Services, Booking, Login, and other essential sections.
- **Hero/Branding Section:** An introductory section with a strong branding message and visuals to communicate the essence of the car wash service.
- **Call-to-Action Button:** A prominent button encouraging users to book a service, redirecting them to the Services page.
- **Featured Services:** Display up to six services with brief descriptions and images to highlight the most popular offerings.
- **Review Section:**
    - **Input Field & Rating Component:**
        - Text area for feedback.
        - Star-based rating system (1-5 stars).
    - **Design:** The review section should be visually appealing, using engaging colors, icons, and animations to encourage users to leave feedback. Drawing inspiration from platforms like Dribble or Pinterest can help create an attractive and interactive design.
    - **Post-Submission Display:**
        - Display overall site's rating (average of submitted ratings).
        - Show last two user reviews with ratings and feedback.
    - **"See All Reviews" Button:** Redirects to the "Reviews" page where the user can see all the reviews.
    - **Redirection:** The user should be redirected to the home page after login, and if possible, directly to the review section on the 
      home page which is optional.
    - Black Overlay with Login Button:
       Display a black overlay above the review section if the user is not logged in.
       Include a "Login" button on the overlay.
      Upon clicking, the user is redirected to the login page.
      After a successful login, redirect the user back to the review section or the home page..
      Conditional Display: If the user is already logged in, the overlay should not be shown.
- **Footer:** Links to relevant pages, contact information, and social media links.

**2. User Authentication Pages**

- **Sign Up Page:**
    - **Form Fields:** Name, email, password, phone number, address.
    - By default, every user will have the "USER" role. Initially, there should be an admin in the database. Later, that admin can promote a user to the "ADMIN" role.
    - **Functionality:**
        - Allows users to create a new account.
        - Form validation (e.g., correct email format).
        - Displays success or error messages based on the outcome.
- **Login Page:**
    - **Form Fields:** Email, password.
    - **Functionality:** Login, token-based authentication, proper error messages.
    - **Please make sure to provide the admin login credentials when submitting the assignment.** 

**3. Services Page**

- **Features:** List of all car wash services with descriptions, prices, and durations.
- **Functionality:** Search, filter, and sort services (e.g., by price, duration).

**4. Service Details Page**

- **Features:** Detailed information about selected services, display available time slots.
    - Detailed information about the selected service.
    - Display available time slots for the selected service on the current date by default.
    - Booked time slots should be disabled and unclickable.
    - Available time slots should be clickable for selection.
    - Optional: A calendar to choose a date, with available slots appearing based on the selected date.
    - A "Book This Service" button appears after selecting a slot.

**5. Booking Page**

- **Features:**
    - **Left Side:** Display the selected service and time slot. Try to make the design attractive.
    - **Right Side:** A form for submitting user information (User name, email, selected time - auto-filled).
    - A "Pay Now" button for payment processing.
- **Functionality:**
    - Upon clicking the "Pay Now" button, the user will be redirected to AAMARPAY, and the slot status associated with the booking will be marked as "booked."
    - Redirects the user to a success page after payment.

**6. Error Pages**

- **Features:** Custom 404 page for non-existent routes.
- **Functionality:** Navigation options to guide users back to safe pages (e.g., Home, Login).

---

### Admin Pages

**1. Admin Dashboard**

- **Features:** Overview of recent bookings, user management, slot management, and service management.
- **Functionality:**
    - Accessible only to admin users.
    - **Service Management:**
        - In the admin dashboard, the service data should be displayed in a tabular format.
        - When implementing the "Add Service" feature, a single "Add Service" button should be provided on the page. Upon clicking this button, a modal containing the service creation form will open. After the user completes and submits the form, the modal will close automatically, and the newly created service will be optimistically updated in the system, providing a real-time experience that enhances the overall user interaction.
        - In each row of the service data table, there should be action buttons for updating and deleting the service data.
        - Upon clicking the update button, the system should either open a modal. The fields within the form should be pre-populated with the selected service data, allowing for a smooth and efficient editing process.
        - Before deleting a service, there should be a confirmation pop-up to ensure that the user intends to proceed with the deletion.
    - **Slot Management:**
        - Ability to create and manage slots for services.
        - An admin should be able to update the slot status individually.
        - An admin should not be able to update the status of a booked slot
        - The admin is authorized to toggle the slot status between AVAILABLE and CANCELLED.
    - **User Management:**
        - View user bookings in a tabular form.
        - User management: view user list, edit user roles.

---

### User Pages

**1. User Dashboard**

- **Features:** Overview of bookings and account information.
- **Functionality:**
    - Update profiles, and manage personal information.
    - **Past Bookings:** Displayed in tabular format.
    - **Upcoming Bookings:** Displayed in card format with a countdown timer.

**2. Service Slot Countdown**

- **Features:** After a user creates a booking, display a countdown timer that shows the time remaining until their selected slot. If multiple slots are selected, only the countdown for the immediate next slot will be shown in the navbar. Additionally, in the user's "Upcoming Bookings," a countdown for each booking will be displayed on the booking card.

---

### Bonus Requirements

- **Service Comparison Feature:** Enable users to select and compare two or more services side by side. This feature should display the services’ features, prices, and durations, helping users make informed decisions.
- **Scroll to Top Button:** Appears on scroll, allows quick return to the top of the page.
- **UI/UX Improvements:** Focus on enhancing the user interface and experience by implementing design best practices, ensuring the application is intuitive, responsive, and visually appealing.
- **GitHub Contributions:** Maintain a well-documented GitHub repository with a minimum of 15 commits. Each commit should represent meaningful progress, such as feature implementation, bug fixes, or UI enhancements.

### Deliverables

- Fully functional frontend application integrated with the backend.
- Responsive design for all pages.
- User and Admin dashboards with described features.
- Complete backend integration.
- Clean, well-organized, and documented code.
- Creative solutions to integration challenges.

**[N.B: If backend updates are needed for Assignment 3 to meet these requirements, please adjust as necessary.]**
