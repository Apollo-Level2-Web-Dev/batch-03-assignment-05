<h1 align="center">4. Bike Rental Service Website</h1>

<h3 align="center">⚠️ Read the entire requirement thoroughly. Every detail must be carefully reviewed from start to finish.</h3>

---


**Objective:**  
Develop a user-friendly, functional frontend for a Bike Rental Booking System. This system should integrate with the backend from **Assignment 3** and provide a seamless user experience with authentication, bike management, booking, and advanced features.

---

#### **Public Pages**

**1. Navbar & Footer**
- **Navbar:**
  - **Logo:** Positioned at the top left, clicking redirects to the home page.
  - **Menu Items:** Links to Home, About Us and other necessary routes that may be conditional based on user role.
  - **Authentication Links:** Login/Sign Up (if not logged in), Logout (if logged in).

- **Footer:**
  - **Social Media Icons:** Links to social profiles.
  - **Website Links:** Privacy Policy, Terms of Service, Contact Us.

**2. Home Page**
- **Hero Section:**
  - **Banner:** Background image or video related to bikes.
  - **Information:** Prominent call-to-action and a search bar for bike availability.

- **Featured Section:**
  - **Available Bikes:** Display bikes with brand names, images, and a "View Detail" button.

- **Testimonials:**
  - **Reviews:** Short quotes from satisfied customers.

- **Why Choose Us:**
  - **Benefits:** Key selling points (e.g., best prices, wide selection, excellent customer service).

- **Coupons & Discounts Section (Bonus):**
  - **Promotions:** Highlight active discounts or coupon codes.
  - **Usage:** Brief instructions on applying coupons.

- **Contact Us Section:**
  - **Form:** Fields for name, email, message, and a submit button.

**3. About Us Page**
**Purpose:** Provide information about the organization.

- **Mission Statement:**
  - **Description:** Platform’s purpose and values.

- **Team Section:**
  - **Profiles:** Photos and bios of key team members.

- **History & Milestones:**
  - **Timeline/Narrative:** Organization’s journey and achievements.

- **Contact Information:**
  - **Details:** Office address, phone number, email.
    
**4. User Authentication**
- **Sign Up Page:**
  - **Form Fields:** Name, Email, Password, Phone, Address.
  - **Validation:** Ensure all fields are correctly filled and required.
  - **Success Redirect:** To login page with a success message.

  _**Note:** By default, every user will have the "USER" role. Initially, there should be an admin in the database. Later, that admin can promote a user to the "ADMIN" role._

- **Login Page:**
  - **Form Fields:** Email, Password.
  - **Validation:** Ensure fields are filled and correct.
  - **Success Redirect:** To dashboard.

- **Protected Dashboard Routes:**
  - **Access Control:** Ensure only authenticated users(Admin/User) can access certain routes.
---

### **User Dashboard [Private/Protected Route]**

**5. User Profile Management**
- **Profile Page:**
  - Welcome Message: Personalized greeting with user’s name.
  -  Display user details such as Name, Email, Phone, Address and if you want you can add other information
  -  Allow users to update their profile information.

**6. Bike Management (public)**

You can keep the Bike List on navbar
- **Bike Listing Page:**
  - **Display:** List of available bikes with necessary information, a View Detail Button
  - **Filter:** Implement filter system to filter bike based on brand, model, availability, etc.
  - **View Detail Button:** Redirects to the Bike Detail Page.

- **Bike Detail Page:**
  - Display detailed information about the selected bike (Description, Price, CC, Year, Brand, Availability and you can other information if you want). There will be a Book Now button. Redirect users to the booking process.
    
Note: If not logged in, users need to log in to book a bike

**7. Rental Management**
- **Booking Process:**
  - **Book Now Button:** On click, open a modal/form with fields like Start Time and a pay button redirecting user to the payment page with advanced payment of tk 100. After successful payment booking will be confirmed. .
  - **Rental Confirmation:** Show a confirmation message and update bike availability.

- **My Rentals Page:**
  - **Tabs:** Implement tab system having two tabs - Paid and Unpaid. By default, the Unpaid Tab will be active
  - **Paid Tab:** List of rentals with details like Bike Name, Start Time, Return Time, and Total Cost.
  - **Unpaid Tab:** Similar to Paid, but includes a "Pay" button.
  - **Pay Button:** Redirect users to the Payment Page.

   **Note:** Upon successful payment, move the rental to the **Paid** tab.

---

### **Admin Pages [Private for Admin Only]**

**8. Admin Profile Management**

- **Profile Page:** Same functionalities described in **User Profile Mangement**.
  
**9. Bike Management**

- **Display:** List of available bikes with necessary information, an update button and a delete button. Add filter system to bikes based on brand, model, availability, etc
  
- **Create/Edit Button:**
  A Create/Edit button when clicked opens a modal.
  - **Fields:** Name, Description, Price, CC, Year, Model, Brand, etc.
  - **Validation:** Ensure all required fields are correctly filled.
    
- **Update Button:**
  - Can update a bike information
  - The fields should be prefilled with existing data so that the admin can update a particular field only..
    
- **Delete Button:**
  - **Confirmation Dialog:** Before bike deletion.

**10. User Management**
- **User Management:**
  - **Actions:** Delete users or promote users to admin.

**11. Return Bike**
- Return Process:
Admins can view a list of rental details and use a "Calculate" button to update status and calculate cost by submitting the end time. The cost will be shown in **Rental page** of the user side.

- Success Handling:
Upon successful return, show a message like "Bike returned successfully" and update the rental status.

**12. Coupon Management: (Bonus)**
- The admin can create and manage all coupon codes.
  
---

#### **Error Handling**
- **Error Messages:**
  - **API Failures:** Display via Toast notifications.
  - **Validation Errors:** Show next to form fields.

- **No Data Handling:**
  - **Friendly Messages:** When no bikes or rentals are available.

- **404 Page:**
  - **Custom Design:** For unmatched routes.

---

#### **UI/UX**
- **UI/UX Quality:**
  - **Design:** Clean, modern, and user-friendly.
  - **Design Principles:** Consistent color schemes and typography.
  - **User Experience:** Smooth navigation and intuitive controls.

- **Responsiveness:**
  - **Cross-Device Compatibility:** Fully responsive on mobile, tablet, and desktop.

---

#### **Bonus Features**
- **Coupon Functionality:**

  - **User Experience:** Coupons will be available in the homepage for users to apply them for a discount on their rentals.
  - **Gamified Feature:** Users can spin a wheel to win discounts of varying percentages, such as 10%, 20%, or 30%.

    **Note:** Once the wheel lands on a discount, a modal will pop up displaying the coupon code associated with the selected discount. The modal will include a "Copy" button, making it easy for users to copy the coupon code. Additionally, the coupon code will automatically appear on the Rental page for the specific rental, ensuring that users can apply their discount seamlessly during the checkout process.

- **Side-by-Side Comparison:**
  - **Comparison Tool:** Allow users to compare multiple bikes, highlighting key features.

- **Micro-Animations:**
  - **Interactive Elements:** Use subtle animations to enhance user experience.

- **Dark Mode:**
  - **Theme Switcher:** Toggle between light and dark mode using TailwindCSS.

---

### **Deliverables**
- Fully functional frontend application integrated with the backend.
- Responsive design for all pages.
- User and Admin dashboards with described features.
- Complete backend integration.
- Clean, well-organized, and documented code.
- Creative solutions to integration challenges.

### **References for Idea Generation**
- **Inspiration Sites:**
  - [Bike Share](https://www.bikeshare.com/)
  - [Spinlister](https://www.spinlister.com/)

**[N.B: If backend updates are needed for Assignment-3 to meet these requirements, please adjust as necessary.]**
