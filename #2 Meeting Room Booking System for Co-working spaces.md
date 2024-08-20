<h1 align="center">2. Meeting Room Booking System for Co-working spaces</h1>

<h3 align="center">⚠️ Read the entire requirement thoroughly. Every detail must be carefully reviewed from start to finish.</h3>

* * *

**Objective:** The goal of this assignment is to integrate the frontend with the backend system developed in **Assignment 3**, which is a meeting room booking platform. You may update your backend as needed for the frontend implementation. This integration will involve creating a fully functional user interface that communicates with the backend via API calls. Additionally, you'll need to add both a user dashboard and an admin dashboard, ensuring a smooth and user-friendly experience for booking meeting room facilities.

# Detailed Requirements:

## Main Requirements:

### 1. **Landing Page:**

*   **Purpose:** Acts as the gateway to the platform, offering a general overview and guiding users to specific actions like booking a room or logging in.
*   **Components:**
    *   **Header:** 
        *   **Logo/System Name:**
            *   Position the logo or system name at the top left of the navbar.
            *   Clicking the logo redirects to the homepage.

  

    *   **Navigation Links:**
            *   **Home:** Redirects to the homepage.
            *   **Meeting Rooms:** Redirects to the Meeting Rooms page showing all available rooms.
            *   **About Us:** Redirects to the About Us page with system and team information.
            *   **Contact Us:** Redirects to the Contact Us page for inquiries and support.
            *   **Login/Register:** Allows users to access their accounts or create a new account.

> Visually distinguish the active link using a different color or underline.

*   **User Icon/Dropdown:**
    *   Display the user's avatar or profile picture on the right side of the navbar after login.
    *   Clicking the user icon opens a dropdown with options like :
        *   _For Authenticated User:_
            *   **My Bookings :** Redirects to the My Bookings page for managing user bookings.
            *   **Logout Button**
        *   _For Admin :_
            *   **Dashboard** : Redirects to the admin dashboard for managing rooms and bookings.
            *   **Logout Button**

  
*    **Hero Section:** 
    *   **Visual Appeal:**
        *   A large banner image or video highlighting a modern workspace.
*   **Headline & Subheadline:**
    *   **Headline:** _Example:_ "Book Your Ideal Meeting Room with Ease" .
    *   **Subheadline:** _Example:_ "Efficient, hassle-free room booking for all your meeting needs."

> Feel free to modify the your site's content with relevant texts. Ignore using lorem texts.

*   **Call to Action (CTA) Button:**
    *   A prominent "Book Now" button that redirects users to the Meeting Rooms page.

  

*    **Service Advertisement Section:**

**Highlighted Services:**

*   **Real-Time Availability:** Up-to-date room availability.
    *   **Instant Booking Confirmation:** Immediate confirmation of bookings.
    *   **Flexible Scheduling:** Options to adjust booking times and dates.
    *   **24/7 Support:** Round-the-clock customer support.

> Feel free to modify the your site's content with relevant texts. Ignore using lorem texts.

  

*    **Featured Rooms Section:**

**Room Cards:**

*   **Image:** High-quality multiple images of featured rooms.
    *   **Room Name:** Display the room name.
    *   **Capacity:** Number of people the room can accommodate.
    *   **PricePerSlot :** Show the price of each slot.
    *   **"See Details" Button:** Takes users to the Room Details page.

> Display at least 6 most popular or newly added rooms, sorted dynamically.

**See More Button:**

*    A button at the bottom of the section linking to the Meeting Rooms page for more options.

  

*   **Extra Sections:**

**Why Choose Us?:**

*    Highlight unique features such as "Seamless Booking Experience" and "Secure Transactions."

**How It Works Section:**

*   **Process Explanation:**
    *   **Step 1:** Select a Room
    *   **Step 2:** Choose Date & Time
    *   **Step 3:** Confirm Booking

> Use icons or illustrations to represent each step for clarity.  
> Feel free to modify the section or its content that is relevant to the niche of the project.

  

*   **Customer Testimonials Section:**

**Carousel Display:**

*   **Profile Picture:** Images of customers giving testimonials.
    *   **Name & Role:** Names and roles of the customers.
    *   **Testimonial Text:** Quotes about their experience with the system.

> Testimonials can be fetched from a database or displayed statically.

  

*   **Footer Section:**

**Contact Information:**

*   Email, phone number, and office address.

**Social Media Links:**

*   Clickable icons for the system's social media profiles.

**Additional Links:**

*   Privacy Policy, Terms of Service, and other relevant pages.

**Design:**

*    Clean and minimalistic design with clear, readable text.

  

### **2\. Dashboard:**

*   **User Dashboard:**
    *   **Purpose:** Allows users to manage their bookings, and access personalized content.
    *   **Components:**
        *   **Welcome Message:** Personalized greeting. **To retrieve user information, develop an API to fetch user data from the database.**
        *   **My Bookings Page \[Private\] :** List of bookings with options to view details, or cancel.
            *   **Display Bookings:**
                *   List user bookings with:
                    *   **Room Name**
                    *   **Date & Time**
                    *   **Status:** (Unconfirmed /Confirmed)

  

*   **Admin Dashboard:**
    *   **Purpose:** Provides administrators with tools to manage facilities, bookings, and users.
    *   **Components:**
        *   **Welcome Message:** Personalized greeting. **To retrieve user information, develop an API to fetch user data from the database.**
        *   **Meeting Room & Slots Management:** Administrators can perform CRUD operations on meeting rooms & slots, including adding new meeting room or slot, editing existing details, and removing rooms or slots. In backend, the meeting room model should be updated to include an "image" field. For image uploads, you can use services like Imgbb, Cloudinary, or static image links.

  

*   **Room Management:**

**Create Room Button:**

*   Button to open a form for adding new rooms with fields for all necessary details.

**Room List Table:**

*   **Table Columns:**
    *   **Room Name**
    *   **Capacity**
    *   **Availability**
    *   **Action Buttons:** (Update/Delete)
*   **Action Buttons:**
    *   **Update Room:**
        *   Opens a modal with a form to update room details (room name, capacity, availability, amenities, image upload etc).
    *   **Delete Room:**
        *   Opens a confirmation modal to confirm room deletion.
    *   **Real-Time Updates:**
        *   Ensure create, updates and deletions reflect immediately with optimistic updates.

  

*   **Slots Management:**
    *   **Create Slot Button:**
        *   Button to open a form for adding new slot with fields for all necessary details.
    *   **Slots List Table:**
        *   **Table Columns:**
            *   **Room Name**
            *   **Room No.**
            *   **Date**
            *   **Start Time**
            *   **End Time**
            *   **Action Buttons:** (Update/Delete)
    *   **Action Buttons:**
        *   **Update Slot:**
            *   Opens a modal with a form to update slot details (room name, date, start time, end time etc ).
        *   **Delete Slot:**
            *   Opens a confirmation modal to confirm slot deletion.
        *   **Real-Time Updates:**
            *   Ensure create, updates and deletions reflect immediately with optimistic updates.

  

*   **Booking Management:**
    *   **Booking List Table:**
        *   **Table Columns:**
            *   **Room Name**
            *   **User Name**
            *   **User Email**
            *   **Date & Time**
            *   **Status:** (Confirmed/Unconfirmed)
            *   **Actions:**
                *   **Approve Booking:** Approve or reject pending bookings with status change options.
                *   **Delete Booking:** Delete bookings with a confirmation modal.

  

###  3. **Login/Registration Page:**

*   **Purpose:** Allows users to access their accounts or create a new account.
*   **Components:**
    *   **Login Form:** Email and password fields.
        *   **Functionality:**
            *   Users can log in to their accounts.
            *   Token-based authentication to maintain user sessions.
            *   Displays error messages for incorrect credentials.

  

    *   **Registration Form:** Fields for name, email, password, phone, role (automatically set to "user"), address and confirmation with a "Sign Up" button.
        *   **Functionality:**
            *   Allows users to create a new account.
            *   Form validation (e.g., correct email format).
            *   Displays success or error messages based on the outcome.

    *   **Social Login:** Option to log in or register using social media accounts (optional).
    *   **Error Handling:** Clear error messages for invalid credentials or registration errors.

  

### 4. **About Us Page:**

*   **Purpose:** Provides information about the organization behind the platform.
*   **Creative Presentation:**
    *   Use animations, gradients, and engaging visuals to make the page attractive.
*   **Components:**
    *   **Mission Statement:** A brief description of the platform's purpose and values.
    *   **Team Section:** Photos and bios of key team members.
    *   **History & Milestones:** Timeline or narrative of the organization's journey and achievements.
    *   **Contact Information:** Office address, phone number, and email.

  

### 5. **Contact Us Page:**

*   **Purpose:** Allows users to get in touch with support or provide feedback.
*   **Design Elements:**
    *   Use basic animations to make the form visually appealing and user-friendly.
*   **Components:**
    *   **Contact Form:** Fields for name, email, subject, and message, with a "Submit" button.
    *   **Map Integration:** An embedded map showing the office location (optional).
    *   **Contact Details:** Phone number, email, and physical address.

  

### 6. Meeting Room **Listing Page:**

*   **Purpose:** Displays a list of all available(based on isDeleted = false) rooms .
*   **Components:**
    *   **Card View Display:**
        *   **Room Name:** Display the room name.
        *   **Capacity:** Number of people the room can accommodate.
        *   **PricePerSlot :** Show the price of each slot.
        *   **"See Details" Button:** Takes users to the Room Details page.
    *   **Search Functionality:**
    *   **Search Bar:**
        *   Allows searching by room name or keyword.
        *   Results update in real-time as the user types.
    *   **Filter Options:**
        *   **Capacity:** Select rooms based on capacity.
        *   **PricePerSlot :** Filter by price per slot
    *   **Sort Options:**
        *   **By PricePerSlot :** Sort by price range per slot
    *   **Clear Filter Button:**
        *   Resets all applied filters to default settings.

  

### 7. **Room Details Page \[Private/Protected Route\] :**

*   **Purpose:** Provides detailed information about a specific room.
*   **Components:**
    *   **Room Information:**
        *   **Room Name:** Display the room name.
        *   **Room No. :** Display the room number.
        *   **Floor No. :** Display the floor number.
        *   **Capacity:** Number of people the room can accommodate.
        *   **PricePerSlot :** Show the price of each slot.
        *   **Amenities :** Show amenities available in the room (e.g., "Projector", "Whiteboard
        *   **Book Now Button:**
            *   A prominent button to start the booking process.
    *   **Booking Button:** A "Book Now" button that navigates to the booking page.

  

### **8\. Booking Page:**

> You can either use separate page or use modal for booking process . If you use a separate route for this, then make sure to keep the route private.

*   **Purpose:** The Booking Page serves as the interface where users can book a specific room and check its availability. It guides the user through selecting a room, checking available time slots, filling out booking details, and completing the booking process, including payment.
*   **Components:**
    *   **Booking Form:**
        *   **Date and Time Selection:**
        *   **Calendar View:**
            *   Allows users to choose a booking date.
        *   **Time Slots:**
            *   Show available time slots for that selected date. (based on isBooked = false)
        *   **User Information Form:**
            *   Name
            *   Email
            *   Phone number
            *   Address

> Auto pre-fill the user input details with the logged in user information.

#### **Confirmation and Payment** / **Checkout Page: \[Private\]**

*   **Booking Summary:** Display a summary of the booking details including room name, date, time, and cost.
    *   **Payment:** Integration with SSL Commerz/AmarPay for secure payment processing.
    *   **Confirm Booking Button:** Finalize the booking after selecting the payment option.
    *   **Confirmation Modal:** Show booking details and a thank you message.

  

### 9. **Error Pages**

*   **Features:** Custom 404 page for when a user navigates to a non-existent route.
*   Custom error messages for unauthorized access (e.g., trying to access admin pages as a regular user).
*   **Functionality:** Navigation options to guide users back to a safe page (e.g., Home, Login).

### **10\. UI/UX:**

*   **Design Principles:** Implement a clean, modern design with consistent color schemes and typography.
*   **User Experience:** sure smooth navigation, intuitive controls, and accessibility considerations.
*   **Responsiveness:** Ensure the website is fully responsive on mobile, tablet, and desktop devices.

## Bonus Requirements

1. **Scroll to Top Button**: Implement a "Scroll to Top" button that becomes visible when users scroll down the page. This button should be easily accessible, allowing users to quickly return to the top of the page with a single click, enhancing navigation and the overall user experience.
2. **Pagination:** Add pagination to the "Meeting Room Listing" page to improve user experience by breaking down content into manageable sections, making it easier for users to browse through facilities.
3. **Error Handling:** Implement consistent error message displays for any API failures using Toast notifications. Ensure that validation error messages are displayed directly on the relevant form fields for better user feedback.
4. **GitHub Contributions:** Maintain a well-documented GitHub repository with at least 15 meaningful commits. Each commit should reflect significant progress, such as feature implementation, bug fixes, or UI enhancements.
5. **Professional README File:** Ensure thorough documentation is available. This should encompass detailed instructions for project setup and execution, alongside pertinent details. **For a structured guide, refer to the** [**Project README File Template**](https://github.com/Apollo-Level2-Web-Dev/batch-03-assignment-05/blob/main/Project%20Documentation%20Template.md)**. Please adhere to this template or follow the** [**Markdown Syntax Guide**](https://github.com/Apollo-Level2-Web-Dev/batch-03-assignment-05/blob/main/Markdown%20Syntax%20Guide.md)**.**

* * *

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

  

### **References for Idea Generation**

*   **Inspiration Sites:**
    *   [https://www.booking.com/](https://www.booking.com/)
    *   [https://www.convene.com/](https://www.convene.com/)