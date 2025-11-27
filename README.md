# EmpowerHer - Gender-Based Violence Reporting Platform

EmpowerHer is a secure, free, and confidential platform designed to help survivors of gender-based violence report incidents, access support services, and track their cases. The platform prioritizes user privacy, security, and provides AI-powered assistance to guide users through their journey.

## 🌟 Features

### 1. **Free & Accessible**
- **No Payment Required**: The platform is completely free to use. No subscriptions, no payment gateways, no barriers to access.
- **Unlimited Reports**: Users can submit as many incident reports as needed without any restrictions.
- **Open Access**: All features are available to all users without premium tiers or limitations.

### 2. **AI-Powered Helpline Assistance**
- **24/7 AI Support**: Get instant, confidential support from our AI assistant
- **Intelligent Responses**: The AI understands context and provides appropriate guidance
- **Resource Recommendations**: Get connected to relevant support services based on your needs
- **Quick Suggestions**: Pre-filled message templates for common scenarios
- **Emergency Guidance**: Immediate direction to emergency services when needed

### 3. **Anonymity Options**
- **Anonymous Reporting**: Submit reports without linking them to your account
- **Privacy Protection**: Your identity remains confidential when you choose anonymous mode
- **Secure Storage**: All reports are encrypted and stored securely
- **OB Number Tracking**: Even anonymous reports receive tracking numbers for case follow-up

### 4. **Comprehensive Audit Trails**
- **Full Transparency**: See exactly when and how your reports were accessed
- **Access History**: Track who viewed your report, when, and from where
- **Status Changes**: Monitor all status updates and case progress
- **Accountability**: Complete audit log for administrative actions
- **User Dashboard**: View audit trails for all your reports in one place

### 5. **Incident Reporting**
- **Detailed Reports**: Comprehensive form to capture all incident details
- **Multiple Incident Types**: Support for various forms of gender-based violence
- **Evidence Documentation**: Record witnesses, evidence, and supporting information
- **Urgency Levels**: Mark reports as low, medium, high, or emergency priority
- **Status Tracking**: Real-time updates on case progress

### 6. **Case Management**
- **OB Number System**: Unique tracking numbers for each report
- **Status Updates**: Receive notifications about case progress
- **Officer Assignment**: Track which officers are handling your case
- **Case Notes**: View public case notes and updates
- **Next Steps**: See upcoming actions and deadlines

### 7. **Support Resources**
- **Helpline Directory**: Access to multiple support services
- **Emergency Contacts**: Quick access to emergency services
- **Legal Aid**: Information about legal support services
- **Medical Support**: Resources for medical care and forensic examination
- **Counseling Services**: Trauma-informed counseling options

### 8. **User Dashboard**
- **Report Overview**: View all your reports in one place
- **Quick Actions**: Easy access to report incidents, view helplines, and more
- **Statistics**: Track your active cases and resolved reports
- **Encouragement Messages**: Words of support and strength

## 🏗️ Architecture

### Technology Stack

**Backend:**
- Node.js with Express.js
- MongoDB with Mongoose
- JWT Authentication
- RESTful API Architecture

**Frontend:**
- Next.js 14 (React Framework)
- TypeScript
- Tailwind CSS
- Framer Motion (Animations)
- React Hook Form (Form Management)
- Zod (Schema Validation)

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

## 🚀 Getting Started

### Prerequisites

- Node.js (v16 or higher)
- MongoDB (local or MongoDB Atlas)
- npm or yarn

### Installation

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

## 📖 How It Works

### User Registration & Authentication

1. **Register**: Users create an account with email and password
2. **Login**: Secure JWT-based authentication
3. **Session Management**: Tokens stored securely in browser

### Reporting an Incident

1. **Access Report Form**: Click "Report Incident" on dashboard
2. **Choose Anonymity**: Option to submit anonymously
3. **Fill Details**: Complete multi-step form with:
   - Personal information (optional if anonymous)
   - Incident details (type, date, time, location)
   - Description and evidence
   - Urgency level
   - Consent options
4. **Submit**: Report is encrypted and stored securely
5. **Receive OB Number**: Unique tracking number for case follow-up

### AI Helpline Assistant

1. **Access Chat**: Click "AI Helpline Assistant" on dashboard
2. **Start Conversation**: Type your message or use quick suggestions
3. **Get Support**: AI provides:
   - Emotional support and validation
   - Resource recommendations
   - Emergency guidance
   - Information about services
4. **View Resources**: Access directory of support services

### Viewing Audit Trails

1. **Access Reports**: View your reports on the dashboard
2. **View Audit Trail**: Click "View Audit Trail" on any report
3. **See History**: View complete log of:
   - Who accessed the report
   - When it was accessed
   - Status changes
   - Case notes added
   - Officer assignments
   - IP addresses (for security)

### Case Management

1. **Status Updates**: Admins update case status
2. **Notifications**: Users see updates in real-time
3. **Officer Assignment**: Cases assigned to specific officers
4. **Case Notes**: Public notes visible to users
5. **Resolution**: Cases marked as resolved when complete

## 🔒 Security Features

- **Encryption**: All data encrypted in transit and at rest
- **JWT Authentication**: Secure token-based authentication
- **Role-Based Access**: Admin, Officer, and User roles
- **Audit Logging**: Complete audit trail for accountability
- **IP Tracking**: Security monitoring through IP logging
- **Anonymous Mode**: Privacy protection for sensitive cases
- **Consent Management**: Explicit consent for data sharing

## 📡 API Endpoints

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - User login
- `GET /api/auth/me` - Get current user

### Reports
- `POST /api/reports` - Submit new report
- `GET /api/reports/:obNumber` - Get report by OB number
- `GET /api/reports/user/my-reports` - Get user's reports
- `PUT /api/reports/:obNumber/status` - Update report status (Admin)

### Helpline
- `POST /api/helpline/chat` - AI chat assistance
- `GET /api/helpline/resources` - Get support resources

### Audit Trails
- `GET /api/audit/reports/:obNumber` - Get audit trail for report
- `GET /api/audit/my-reports` - Get audit trails for user's reports
- `GET /api/audit/all` - Get all audit trails (Admin)

### Admin
- `GET /api/admin/dashboard` - Admin dashboard stats
- `GET /api/admin/reports` - Get all reports
- `GET /api/admin/reports/:obNumber` - Get report details
- `PUT /api/admin/reports/:obNumber/status` - Update report status

## 🎯 Use Cases

### For Survivors
- Report incidents safely and confidentially
- Track case progress in real-time
- Access AI-powered support 24/7
- View complete audit trail of report access
- Submit reports anonymously if needed

### For Administrators
- Manage all reports from dashboard
- Assign cases to officers
- Update case status and add notes
- View comprehensive audit trails
- Monitor system activity

### For Officers
- Access assigned cases
- Update case progress
- Add case notes
- Communicate with survivors

## 🔄 Workflow Example

1. **User registers** → Account created
2. **User submits report** → OB number generated
3. **Report appears in admin dashboard** → Admin reviews
4. **Admin assigns officer** → Case assigned
5. **Officer updates status** → User sees update
6. **Case progresses** → Status updates tracked
7. **Case resolved** → Marked as complete
8. **User views audit trail** → Sees complete history

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

## 📝 Environment Variables

### Backend Required Variables
- `MONGODB_URI` - MongoDB connection string
- `JWT_SECRET` - Secret key for JWT tokens
- `PORT` - Server port (default: 5000)
- `FRONTEND_URL` - Frontend URL for CORS
- `NODE_ENV` - Environment (development/production)

### Frontend Required Variables
- `NEXT_PUBLIC_API_URL` - Backend API URL

## 🤝 Contributing

This is a platform for supporting survivors of gender-based violence. Contributions should prioritize:
- User safety and privacy
- Accessibility
- Security
- User experience

## 📄 License

MIT License - See LICENSE file for details

## 🆘 Support

For technical support or questions:
- Check the documentation
- Review API endpoints
- Contact the development team

## 🙏 Acknowledgments

Built with care for survivors of gender-based violence. This platform aims to provide a safe, secure, and supportive environment for reporting incidents and accessing help.

---

**Remember**: If you're in immediate danger, call **1195** or your local emergency number right away.

