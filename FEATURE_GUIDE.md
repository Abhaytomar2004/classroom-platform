# 🎮 SikshaLink Feature Guide

Complete guide to all features available in SikshaLink Classroom Platform.

## 📋 Table of Contents
- [Dashboard](#-dashboard)
- [Authentication](#-authentication) 
- [Live Classes](#-live-classes)
- [Assignments](#-assignments)
- [Resources](#-resources)
- [Attendance](#-attendance)
- [Payment System](#-payment-system)
- [Mentorship](#-mentorship)
- [Notifications](#-notifications)

---

## 🏠 Dashboard

### Student Dashboard
**Features:**
- Personalized welcome with user name
- Quick stats overview (courses, assignments, progress)
- Upcoming classes schedule
- Pending assignments
- Recent activity feed
- Quick access to all major sections

**How to Access:**
1. Login as student
2. You'll be redirected to dashboard automatically
3. Use sidebar navigation for different sections

![Student Dashboard](documentation-screenshots/features/student-dashboard.png)

### Teacher Dashboard
**Features:**
- Class management overview
- Student performance analytics
- Assignment creation quick access
- Schedule management
- Resource upload statistics

**How to Access:**
1. Login as teacher
2. Dashboard shows teaching statistics
3. Create new classes/assignments from quick actions

---

## 🔐 Authentication

### User Registration
**Steps:**
1. Click "Sign Up" on homepage
2. Fill registration form:
   - Full Name
   - Email Address
   - Password (minimum 6 characters)
   - Role (Student/Teacher)
3. Click "Create Account"
4. Automatic login after successful registration

**Features:**
- Form validation
- Password strength indicator
- Role-based access after registration
- Automatic JWT token generation

### User Login
**Steps:**
1. Click "Sign In" on homepage
2. Enter email and password
3. Click "Sign In"
4. Redirected to role-specific dashboard

**Security Features:**
- JWT token-based authentication
- Secure password hashing (bcrypt)
- Automatic token refresh
- Session management

![Login Page](documentation-screenshots/features/login-page.png)

---

## 🎥 Live Classes

### Schedule a Class (Teachers)
**Steps:**
1. Navigate to "Classes" section
2. Click "Schedule New Class"
3. Fill class details:
   - Class Title
   - Description
   - Date & Time
   - Duration
   - Subject/Category
   - Maximum attendees
4. Click "Create Class"

**Features:**
- Calendar integration
- Automatic notifications to enrolled students
- Class capacity management
- Recording options (if integrated)

### Join a Class (Students)
**Steps:**
1. Go to "My Classes" section
2. View upcoming classes
3. Click "Join Class" 5 minutes before start time
4. Enter virtual classroom

**Features:**
- One-click join
- Attendance auto-marking
- Chat and Q&A during class
- Resource sharing during session

---

## 📝 Assignments

### Create Assignment (Teachers)
**Steps:**
1. Navigate to "Assignments" → "Create New"
2. Fill assignment details:
   - Title and Description
   - Due Date
   - Maximum Marks
   - Submission Type (File/Text)
   - Attach resources (optional)
3. Assign to specific class/students
4. Publish assignment

**Features:**
- Rich text editor for instructions
- File attachment support
- Automatic due date reminders
- Plagiarism check integration

### Submit Assignment (Students)
**Steps:**
1. Go to "My Assignments"
2. View pending assignments
3. Click "Submit Assignment"
4. Upload files or write text response
5. Click "Submit"

**Features:**
- File type validation
- Submission history
- Late submission handling
- Teacher feedback system

![Assignments Page](documentation-screenshots/features/assignments-page.png)

---

## 📚 Resources

### Upload Resources (Teachers)
**Steps:**
1. Go to "Resources" section
2. Click "Upload New Resource"
3. Select file(s) or add link
4. Add description and tags
5. Choose visibility (Class/Public)
6. Click "Upload"

**Supported Formats:**
- 📄 PDF, DOC, DOCX
- 🎬 MP4, AVI (video lectures)
- 🖼️ JPG, PNG (images)
- 📊 PPT, XLS (presentations)
- 🔗 External links

### Access Resources (Students)
**Steps:**
1. Navigate to "Resources"
2. Filter by subject/teacher
3. Search by keywords
4. Download or view resources
5. Bookmark important resources

**Features:**
- Advanced search and filtering
- Download statistics
- Rating and review system
- Organized by subjects/categories

---

## ✅ Attendance

### Mark Attendance (Teachers)
**Steps:**
1. Go to "Attendance" section
2. Select class and date
3. View student list
4. Mark Present/Absent/Late
5. Save attendance

**Features:**
- Bulk attendance marking
- Automatic class-wise organization
- Attendance reports generation
- Export to Excel/PDF

### View Attendance (Students)
**Steps:**
1. Navigate to "My Attendance"
2. Select time period
3. View attendance percentage
4. Check detailed daily records

**Features:**
- Visual attendance charts
- Percentage calculations
- Absence reason tracking
- Parent portal integration

---

## 💳 Payment System

### Fee Payment (Students/Parents)
**Steps:**
1. Go to "Payments" section
2. View pending fees
3. Click "Pay Now"
4. Select payment method:
   - Credit/Debit Card
   - UPI
   - Net Banking
   - Digital Wallet
5. Enter payment details
6. Confirm payment

### Payment Methods Available

#### 💳 Card Payments
- Visa, MasterCard, RuPay support
- Secure tokenization
- 3D Secure authentication

#### 📱 UPI Payments
- All major UPI apps supported
- QR code generation
- Instant verification

#### 🌐 Net Banking
- 50+ banks supported
- Secure redirect flow
- Instant confirmation

#### 👛 Digital Wallets
- Paytm, PhonePe, Google Pay
- Quick payment processing
- Wallet balance check

### Test Cards for Development

| Card Number | Type | Scenario | Result |
|-------------|------|----------|---------|
| `4111 1111 1111 1111` | Visa | Normal transaction | ✅ Success |
| `4000 0000 0000 0002` | Visa | Insufficient funds | ❌ Failed |
| `5555 5555 5555 4444` | MasterCard | Normal transaction | ✅ Success |
| `3400 0000 0000 009` | American Express | Normal transaction | ✅ Success |

### Payment Features
- **Smart Payment Selection**: Visual method selector with availability status
- **Custom Amount Input**: Enter any amount between ₹100-₹5,00,000
- **Method-Specific UI**: Dynamic interface based on selected payment method
- **Transaction History**: Complete payment records with receipts
- **Installment Support**: Flexible payment plans available
- **Real-time Processing**: Live payment status updates

![Payment Interface](documentation-screenshots/features/payment-interface.png)

---

## 👨‍🏫 Mentorship

### Find a Mentor (Students)
**Steps:**
1. Go to "Mentorship" section
2. Browse available mentors
3. Filter by subject/expertise
4. View mentor profiles and ratings
5. Send mentorship request

### Become a Mentor (Teachers/Seniors)
**Steps:**
1. Navigate to "Mentorship" → "Become Mentor"
2. Set up mentor profile
3. Define expertise areas
4. Set availability schedule
5. Start receiving requests

**Features:**
- Mentor-student matching algorithm
- Session scheduling
- Progress tracking
- Feedback and rating system
- Video call integration

---

## 🔔 Notifications

### Notification Types
**📅 Schedule Notifications**
- Upcoming class reminders
- Assignment due dates
- Payment deadlines

**🎯 Activity Notifications**
- New assignment posted
- Grade updates
- Resource uploads
- Mentorship requests

**💰 Payment Notifications**
- Payment success/failure
- Fee due reminders
- Receipt generation

### Notification Settings
**Customization Options:**
- Email notifications
- Push notifications
- SMS alerts (premium)
- Frequency control
- Category-wise toggles

**How to Manage:**
1. Go to "Settings" → "Notifications"
2. Toggle notification types
3. Set preferred channels
4. Save preferences

---

## 🛠️ Advanced Features

### Analytics & Reports
**For Teachers:**
- Student performance analytics
- Attendance trends
- Assignment submission rates
- Class engagement metrics

**For Administrators:**
- Platform usage statistics
- Revenue reports
- User growth analytics
- Feature adoption rates

### Multi-language Support
**Available Languages:**
- English (default)
- Hindi (भारत)
- More languages coming soon

**How to Change:**
1. Go to "Settings" → "Language"
2. Select preferred language
3. Interface updates instantly

### Mobile Responsive
**Platform Accessibility:**
- 📱 Mobile phones (optimized)
- 💻 Tablets (responsive)
- 🖥️ Desktop (full features)
- 🌐 Progressive Web App (PWA)

---

## ❓ Frequently Asked Questions

### Q: How do I reset my password?
**A:** Click "Forgot Password" on login page, enter email, check inbox for reset link.

### Q: Can I download class recordings?
**A:** Yes, if teacher has enabled recording download permission.

### Q: How are payments secured?
**A:** We use PCI-DSS compliant payment gateways with SSL encryption.

### Q: Can parents access the platform?
**A:** Yes, parents can have linked accounts to monitor student progress.

### Q: Is there a mobile app?
**A:** Currently web-based with PWA support. Native apps coming soon.

---

## 🆘 Need Help?

- 📖 Check our [Setup Guide](./SETUP_GUIDE.md) for installation help
- 🐛 [Report Issues](https://github.com/ratna-jaiswal/classroom-platform/issues) on GitHub
- 💬 [Join Community](https://github.com/ratna-jaiswal/classroom-platform/discussions) for discussions
- 📧 Email support: [Add support email]

---

**🎉 Explore all features and make the most of SikshaLink platform!**