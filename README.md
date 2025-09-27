# Wellness Waves 🌊

 Empowering Mental Health in the Workplace

A comprehensive employee wellness platform that provides confidential mental health support, live sessions with experts, personalized well-being journeys, and analytics for workplace wellness programs.


 🌟 Features

 🧠 **Mental Health Support**
- **Confidential Therapy & Coaching**: Professional support tailored to individual needs
- **Expert-led Live Sessions**: Interactive group sessions with mental health professionals
- **One-on-One Sessions**: Private consultations with certified therapists
- **Crisis Support**: Immediate assistance when needed

 🔒 **Privacy & Security**
- **100% Confidential**: Personal information never shared with employers
- **Anonymized Data**: Employers only see aggregated company wellness metrics
- **Secure Platform**: End-to-end encryption for all communications
- **GDPR Compliant**: Full data protection compliance

 📊 **Analytics & Insights**
- **Wellness Dashboard**: Track personal progress and goals
- **Company Analytics**: Aggregate wellness metrics for HR teams
- **Progress Tracking**: Monitor engagement and improvement over time
- **Custom Reports**: Detailed insights into wellness program effectiveness

 💳 **Credit System**
- **Flexible Credits**: Use credits for various wellness services
- **Automatic Allocation**: Regular credit distribution to employees
- **Usage Tracking**: Monitor credit utilization and engagement

 🚀 Tech Stack

 Frontend
- **React 18** with TypeScript
- **Tailwind CSS** for styling
- **Material-UI Components** for enhanced UX
- **Framer Motion** for animations
- **Recharts** for data visualization
- **React Hook Form** for form management

 Backend
- **Node.js** with Express.js
- **MongoDB** with Mongoose ODM
- **JWT Authentication** with secure cookies
- **Nodemailer** for email notifications
- **Microsoft Teams Integration** for video sessions
- **bcryptjs** for password hashing

 Infrastructure
- **RESTful API** architecture
- **CORS** enabled for cross-origin requests
- **File Upload** support with Multer
- **Environment Configuration** with dotenv
- **Error Handling** middleware

🛠️ Installation & Setup

 Prerequisites
- Node.js (v18 or higher)
- MongoDB database
- SMTP email service
- Microsoft Teams API credentials (optional)


### 1. Install Dependencies
```bash
npm install
```

### 2. Environment Configuration
Create a `.env` file in the root directory:

```env
# Database
MONGO=your_mongodb_connection_string

# JWT
JWT_SECRET=your_jwt_secret_key

# Domain Configuration
ALLOWED_COMPANY_DOMAINS=company.com,organization.org

# Microsoft Teams (Optional)
MICROSOFT_TEAMS_USER_ID=your_teams_user_id

# Server
PORT=5000
NODE_ENV=development
```

### 4. Start the Application
```bash
# Development mode
npm run dev

# Production mode
npm run build
npm start
```

The application will be available at `http://localhost:5000`

## 📱 Usage

### For Employees
1. **Sign Up**: Register with company email and verify OTP
2. **Set Password**: Create secure login credentials
3. **Dashboard**: Access wellness resources and track progress
4. **Book Sessions**: Schedule live sessions or one-on-one consultations
5. **Track Progress**: Monitor wellness journey and achievements

### For HR/Administrators
1. **Analytics Dashboard**: View company-wide wellness metrics
2. **Usage Reports**: Track platform engagement and effectiveness
3. **Resource Management**: Manage available wellness programs
4. **Privacy Compliance**: Ensure all data remains confidential

## 🔐 API Endpoints

### Authentication
- `POST /api/sign-up` - Employee registration
- `POST /api/verify-otp` - Email verification
- `POST /api/set-password` - Password creation
- `POST /api/sign-in` - Employee login
- `POST /api/send-otp-reset` - Password reset OTP
- `POST /api/reset-password` - Password reset

### Sessions
- `POST /api/live-sessions/book` - Book live group session
- `POST /api/expert-session/book` - Book one-on-one session
- `GET /api/live-sessions/:email` - Get user's booked sessions
- `POST /api/live-sessions/:email/cancel/:id` - Cancel session

### User Management
- `GET /api/employee/profile` - Get user profile
- `PUT /api/employee/update/:id` - Update profile
- `POST /api/update-credits` - Manage user credits

### Analytics
- `GET /api/barchart/data` - Get chart data
- `POST /api/barchart/update` - Update analytics
- `GET /api/notifications` - Get notifications
- `POST /api/notifications` - Create notification

## 🎨 Key Components

### Frontend Components
- **LiveSession**: Interactive live session booking interface
- **Dashboard**: Personal wellness analytics and progress
- **Authentication**: Secure sign-up and sign-in flows
- **Profile Management**: User profile and settings
- **Session Management**: Book, view, and cancel sessions

### Backend Features
- **OTP Verification**: Secure email-based verification
- **Credit System**: Flexible credit allocation and tracking
- **Session Management**: Complete booking and scheduling system
- **Email Notifications**: Automated email communications
- **Data Analytics**: Comprehensive wellness metrics

## 📧 Email Templates

The platform includes beautifully designed email templates for:
- Welcome messages with onboarding information
- OTP verification codes
- Session confirmations and reminders
- Password reset instructions
- Wellness tips and updates

## 🔒 Security Features

- **JWT Authentication** with secure HTTP-only cookies
- **Password Hashing** using bcryptjs
- **OTP Verification** for email security
- **CORS Protection** for API security
- **Input Validation** and sanitization
- **Rate Limiting** for API endpoints

## 🌈 UI/UX Features

- **Responsive Design** for all device types
- **Dark/Light Mode** support
- **Smooth Animations** with Framer Motion
- **Intuitive Navigation** and user flows
- **Accessibility** compliance
- **Professional Branding** with consistent design system

## 🚀 Deployment

### Replit Deployment (Recommended)
1. Fork this repository on Replit
2. Configure environment variables in Replit Secrets
3. Run the application using the Run button
4. Your app will be automatically deployed and accessible

### Manual Deployment
1. Build the application: `npm run build`
2. Set production environment variables
3. Start the server: `npm start`
4. Configure reverse proxy (nginx) if needed

## 🤝 Contributing

We welcome contributions to Wellness Waves! Please follow these steps:

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Commit your changes: `git commit -m 'Add amazing feature'`
4. Push to the branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

### Development Guidelines
- Follow TypeScript best practices
- Use ESLint and Prettier for code formatting
- Write tests for new features
- Update documentation as needed

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Mental health professionals who provided guidance
- Open source community for amazing tools and libraries
- Companies prioritizing employee wellness

**Made with ❤️ for employee wellness**

*Wellness Waves - Where mental health meets technology*
