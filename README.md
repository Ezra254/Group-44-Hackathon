# 💜 EmpowerHer - Gender-Based Violence Reporting Platform

> **Empowering Victims, Accelerating Justice**

EmpowerHer is a secure, free, and confidential platform designed to help survivors of gender-based violence report incidents, access support services, and track their cases. The platform prioritizes user privacy, security, and provides AI-powered assistance to guide users through their journey.

🌐 **Live Application**: [https://empowerhercom.vercel.app/](https://empowerhercom.vercel.app/)  
🔧 **API Endpoint**: [https://group-44-hackathon.onrender.com](https://group-44-hackathon.onrender.com)

---

## ✨ Key Features

### 🆓 **100% Free & Accessible**
- ✅ **No Payment Required**: The platform is completely free to use. No subscriptions, no payment gateways, no barriers to access.
- ✅ **Unlimited Reports**: Users can submit as many incident reports as needed without any restrictions.
- ✅ **Open Access**: All features are available to all users without premium tiers or limitations.

### 🤖 **AI-Powered Helpline Assistance**
- 💬 **24/7 AI Support**: Get instant, confidential support from our AI assistant
- 🧠 **Intelligent Responses**: The AI understands context and provides appropriate guidance
- 📚 **Resource Recommendations**: Get connected to relevant support services based on your needs
- ⚡ **Quick Suggestions**: Pre-filled message templates for common scenarios
- 🚨 **Emergency Guidance**: Immediate direction to emergency services when needed

### 🎭 **Anonymity Options**
- 🔒 **Anonymous Reporting**: Submit reports without linking them to your account
- 🛡️ **Privacy Protection**: Your identity remains confidential when you choose anonymous mode
- 🔐 **Secure Storage**: All reports are encrypted and stored securely
- 📋 **OB Number Tracking**: Even anonymous reports receive tracking numbers for case follow-up

### 📊 **Comprehensive Audit Trails**
- 👁️ **Full Transparency**: See exactly when and how your reports were accessed
- 📝 **Access History**: Track who viewed your report, when, and from where
- 🔄 **Status Changes**: Monitor all status updates and case progress
- ✅ **Accountability**: Complete audit log for administrative actions
- 📱 **User Dashboard**: View audit trails for all your reports in one place

### 📝 **Incident Reporting**
- 📋 **Detailed Reports**: Comprehensive form to capture all incident details
- 🎯 **Multiple Incident Types**: Support for various forms of gender-based violence
- 📸 **Evidence Documentation**: Record witnesses, evidence, and supporting information
- ⚠️ **Urgency Levels**: Mark reports as low, medium, high, or emergency priority
- 📈 **Status Tracking**: Real-time updates on case progress

### 🏛️ **Case Management**
- 🔢 **OB Number System**: Unique tracking numbers for each report
- 📢 **Status Updates**: Receive notifications about case progress
- 👮 **Officer Assignment**: Track which officers are handling your case
- 📄 **Case Notes**: View public case notes and updates
- ✅ **Next Steps**: See upcoming actions and deadlines

### 🆘 **Support Resources**
- 📞 **Helpline Directory**: Access to multiple support services
- 🚨 **Emergency Contacts**: Quick access to emergency services
- ⚖️ **Legal Aid**: Information about legal support services
- 🏥 **Medical Support**: Resources for medical care and forensic examination
- 💚 **Counseling Services**: Trauma-informed counseling options

### 📱 **User Dashboard**
- 📊 **Report Overview**: View all your reports in one place
- ⚡ **Quick Actions**: Easy access to report incidents, view helplines, and more
- 📈 **Statistics**: Track your active cases and resolved reports
- 💜 **Encouragement Messages**: Words of support and strength

---

## 🚀 Quick Start

### 🌐 **Using the Live Application**

1. **Visit the Platform**: Go to [https://empowerhercom.vercel.app/](https://empowerhercom.vercel.app/)
2. **Create an Account**: Click "Sign Up" to create your free account
3. **Start Reporting**: Click "Report Incident" to submit your first report
4. **Get Support**: Access the AI Helpline Assistant for 24/7 support
5. **Track Progress**: View your reports and audit trails from your dashboard

### 💻 **For Developers - Local Setup**

#### Prerequisites

- Node.js (v16 or higher)
- MongoDB (local or MongoDB Atlas)
- npm or yarn

#### Installation Steps

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd EmpowerHer
   ```

2. **Install backend dependencies**
   ```bash
   cd backend
   npm install
   ```

3. **Install frontend dependencies**
   ```bash
   cd ../frontend
   npm install
   ```

4. **Configure environment variables**

   **Backend** (`backend/.env`):
   ```env
   PORT=5000
   MONGODB_URI=mongodb://localhost:27017/empowerher
   JWT_SECRET=your-secret-key-here
   FRONTEND_URL=http://localhost:3000
   NODE_ENV=development
   ```

   **Frontend** (`frontend/.env.local`):
   ```env
   NEXT_PUBLIC_API_URL=http://localhost:5000/api
   ```

5. **Start MongoDB**
   ```bash
   # If using local MongoDB
   mongod
   ```

6. **Start the backend server**
   ```bash
   cd backend
   npm run dev
   ```

7. **Start the frontend development server**
   ```bash
   cd frontend
   npm run dev
   ```

8. **Access the application**
   - Frontend: http://localhost:3000
   - Backend API: http://localhost:5000

---

## 📖 How It Works

### 👤 **For Survivors**

#### 1. **Getting Started**
   - Create a free account at [https://empowerhercom.vercel.app/](https://empowerhercom.vercel.app/)
   - No payment information required
   - Complete privacy protection

#### 2. **Reporting an Incident**
   - Click "Report Incident" on your dashboard
   - Choose to report anonymously or with your account
   - Fill out the comprehensive form:
     - Personal information (optional if anonymous)
     - Incident details (type, date, time, location)
     - Description and evidence
     - Urgency level
     - Consent options
   - Submit your report securely
   - Receive a unique OB number for tracking

#### 3. **Using AI Helpline Assistant**
   - Click "AI Helpline Assistant" on your dashboard
   - Start a conversation with our AI support
   - Get instant guidance, resources, and support
   - Access emergency contacts when needed
   - Use quick suggestion buttons for common questions

#### 4. **Tracking Your Case**
   - View all your reports on the dashboard
   - See real-time status updates
   - Check assigned officers and case notes
   - View complete audit trail of who accessed your report
   - Monitor case progress from submission to resolution

#### 5. **Viewing Audit Trails**
   - Click "View Audit Trail" on any report
   - See complete history of:
     - Who accessed your report
     - When it was accessed
     - Status changes
     - Case notes added
     - Officer assignments
   - Full transparency and accountability

### 👨‍💼 **For Administrators**

1. **Dashboard Access**: View all reports and statistics
2. **Case Management**: Assign officers, update statuses
3. **Audit Monitoring**: View complete system audit trails
4. **User Management**: Manage user accounts and permissions

### 👮 **For Officers**

1. **Assigned Cases**: View cases assigned to you
2. **Update Progress**: Add status updates and case notes
3. **Communication**: Track interactions with survivors
4. **Case Resolution**: Mark cases as resolved when complete

---

## 🏗️ Architecture

### Technology Stack

**Backend:**
- 🟢 Node.js with Express.js
- 🍃 MongoDB with Mongoose
- 🔐 JWT Authentication
- 🌐 RESTful API Architecture

**Frontend:**
- ⚛️ Next.js 14 (React Framework)
- 📘 TypeScript
- 🎨 Tailwind CSS
- ✨ Framer Motion (Animations)
- 📝 React Hook Form (Form Management)
- ✅ Zod (Schema Validation)

### Project Structure

```
EmpowerHer/
├── backend/
│   ├── src/
│   │   ├── models/          # Database models (User, Report, AuditTrail)
│   │   ├── routes/           # API routes (auth, reports, admin, helpline, audit)
│   │   ├── middleware/       # Authentication middleware
│   │   └── server.js         # Express server setup
│   └── package.json
├── frontend/
│   ├── components/          # React components
│   │   ├── ReportModal.tsx
│   │   ├── AIHelplineChat.tsx
│   │   └── AuditTrailView.tsx
│   ├── pages/               # Next.js pages
│   │   ├── dashboard.tsx
│   │   ├── login.tsx
│   │   └── register.tsx
│   └── package.json
└── README.md
```

---

## 📡 API Documentation

### Base URL
**Production**: `https://group-44-hackathon.onrender.com/api`  
**Development**: `http://localhost:5000/api`

### Authentication Endpoints
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - User login
- `GET /api/auth/me` - Get current user

### Reports Endpoints
- `POST /api/reports` - Submit new report
- `GET /api/reports/:obNumber` - Get report by OB number
- `GET /api/reports/user/my-reports` - Get user's reports
- `PUT /api/reports/:obNumber/status` - Update report status (Admin)

### Helpline Endpoints
- `POST /api/helpline/chat` - AI chat assistance
- `GET /api/helpline/resources` - Get support resources

### Audit Trail Endpoints
- `GET /api/audit/reports/:obNumber` - Get audit trail for report
- `GET /api/audit/my-reports` - Get audit trails for user's reports
- `GET /api/audit/all` - Get all audit trails (Admin)

### Admin Endpoints
- `GET /api/admin/dashboard` - Admin dashboard stats
- `GET /api/admin/reports` - Get all reports
- `GET /api/admin/reports/:obNumber` - Get report details
- `PUT /api/admin/reports/:obNumber/status` - Update report status

### Health Check
- `GET /api/health` - API health status

---

## 🔒 Security Features

- 🔐 **Encryption**: All data encrypted in transit and at rest
- 🎫 **JWT Authentication**: Secure token-based authentication
- 👥 **Role-Based Access**: Admin, Officer, and User roles
- 📋 **Audit Logging**: Complete audit trail for accountability
- 🌐 **IP Tracking**: Security monitoring through IP logging
- 🎭 **Anonymous Mode**: Privacy protection for sensitive cases
- ✅ **Consent Management**: Explicit consent for data sharing
- 🛡️ **CORS Protection**: Secure cross-origin resource sharing

---

## 🎯 Use Cases

### 📱 **For Survivors**
- ✅ Report incidents safely and confidentially
- ✅ Track case progress in real-time
- ✅ Access AI-powered support 24/7
- ✅ View complete audit trail of report access
- ✅ Submit reports anonymously if needed
- ✅ Get connected to support services

### 👨‍💼 **For Administrators**
- ✅ Manage all reports from dashboard
- ✅ Assign cases to officers
- ✅ Update case status and add notes
- ✅ View comprehensive audit trails
- ✅ Monitor system activity
- ✅ Generate reports and statistics

### 👮 **For Officers**
- ✅ Access assigned cases
- ✅ Update case progress
- ✅ Add case notes
- ✅ Communicate with survivors
- ✅ Track case resolution

---

## 🔄 Complete Workflow Example

1. **User visits** [https://empowerhercom.vercel.app/](https://empowerhercom.vercel.app/) → Creates account
2. **User submits report** → OB number generated (e.g., OB-12345678-ABCD)
3. **Report appears in admin dashboard** → Admin reviews case
4. **Admin assigns officer** → Case assigned to specific officer
5. **Officer updates status** → User sees real-time update
6. **Case progresses** → Multiple status updates tracked
7. **Case resolved** → Marked as complete
8. **User views audit trail** → Sees complete history of access and changes

---

## 📊 The Scale of Gender-Based Violence

> **Together, we can make a difference**

- **1 in 3** women globally affected by GBV
- **70%** of cases go unreported
- **24/7** support available through EmpowerHer

---

## 🛠️ Development

### Running Tests
```bash
cd backend
npm test
```

### Building for Production
```bash
# Backend
cd backend
npm run build

# Frontend
cd frontend
npm run build
npm start
```

### Creating Admin User
```bash
cd backend
npm run create-admin
```

---

## 📝 Environment Variables

### Backend Required Variables
- `MONGODB_URI` - MongoDB connection string
- `JWT_SECRET` - Secret key for JWT tokens
- `PORT` - Server port (default: 5000)
- `FRONTEND_URL` - Frontend URL for CORS
- `NODE_ENV` - Environment (development/production)

### Frontend Required Variables
- `NEXT_PUBLIC_API_URL` - Backend API URL

---

## 🌟 Why EmpowerHer?

### ✅ **Completely Free**
No hidden costs, no subscriptions, no payment barriers. Everyone deserves access to justice.

### 🤖 **AI-Powered Support**
24/7 intelligent assistance to guide you through difficult times and connect you with resources.

### 🔒 **Privacy First**
Anonymous reporting options and complete audit trails ensure your privacy and transparency.

### 📊 **Full Transparency**
See exactly who accessed your report and when, ensuring accountability at every step.

### 🚀 **Easy to Use**
Simple, intuitive interface designed for ease of use during difficult times.

---

## 🤝 Contributing

This is a platform for supporting survivors of gender-based violence. Contributions should prioritize:
- 🛡️ User safety and privacy
- ♿ Accessibility
- 🔒 Security
- 💜 User experience

---

## 📄 License

MIT License - See LICENSE file for details

---

## 🆘 Support & Resources

### Emergency Contacts
- **Emergency Services**: 1195
- **GVRC Hotline**: +254 719 638 006
- **24/7 Support**: Available through the platform

### Platform Support
- **Email**: support@empowerher.org
- **Help Center**: Available in the application
- **AI Assistant**: 24/7 support through the dashboard

### Additional Resources
- Emergency Contacts
- Legal Support
- Counseling Services
- Medical Support

---

## 🙏 Acknowledgments

Built with care for survivors of gender-based violence. This platform aims to provide a safe, secure, and supportive environment for reporting incidents and accessing help.

**Remember**: If you're in immediate danger, call **1195** or your local emergency number right away.

---

## 🔗 Quick Links

- 🌐 **Live Application**: [https://empowerhercom.vercel.app/](https://empowerhercom.vercel.app/)
- 🔧 **API Endpoint**: [https://group-44-hackathon.onrender.com](https://group-44-hackathon.onrender.com)
- 📡 **API Health Check**: [https://group-44-hackathon.onrender.com/api/health](https://group-44-hackathon.onrender.com/api/health)

---

<div align="center">

**💜 Empowering Victims, Accelerating Justice 💜**

Made with ❤️ for survivors everywhere

</div>
