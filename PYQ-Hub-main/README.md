# PYQ Hub - Previous Year Questions Platform

A modern web application for sharing and accessing Previous Year Questions (PYQs) with AI-powered features and Firebase backend integration.

## 🚀 Features

### Core Features
- **Smart Upload System** - Upload PYQs with automatic categorization
- **Advanced Search** - Find questions by college, course, year, topic, and difficulty
- **AI Question Matching** - Discover similar questions automatically
- **Dashboard** - User-friendly dashboard with statistics and activity tracking
- **Dark Mode** - Toggle between light and dark themes
- **Responsive Design** - Works on all devices

### Technical Features
- **Firebase Integration** - Authentication, Storage, and Firestore database
- **File Upload** - Support for PDF, JPG, PNG files (max 10MB)
- **Real-time Updates** - Live data synchronization
- **Security** - User authentication and file validation
- **Modern UI/UX** - Clean, intuitive interface

## 📁 File Structure

```
PYQ-Hub-main/
├── index.html              # Main landing page
├── dashboard.html          # User dashboard
├── login.html             # Login page
├── signup.html            # Registration page
├── style.css              # Main stylesheet
├── script.js              # Main JavaScript
├── firebase-login.js      # Firebase authentication
├── firebase-upload.js     # Firebase upload functionality
├── loginsignup.css        # Login/signup styles
├── test-auth.html         # Authentication test page
└── pyq logo.jpg          # Application logo
```

## 🔧 Setup Instructions

### 1. Firebase Configuration
The application uses Firebase for backend services. The configuration is already set up in the Firebase files:

- **Authentication**: Email/password login
- **Storage**: File uploads (PDF, JPG, PNG)
- **Firestore**: Metadata storage

### 2. Running the Application
1. Open `index.html` in a web browser
2. Navigate to the dashboard or upload section
3. Sign up/login to access upload features

### 3. Upload Process
1. Click "Upload PYQ" button
2. Fill in the required information:
   - Title
   - Description (optional)
   - College
   - Course
   - Subject
   - Year
   - Semester
   - Exam Type
3. Select a file (PDF, JPG, PNG, max 10MB)
4. Click "Upload & Process"

## 🎯 Key Components

### Upload Modal
- **Form Fields**: Complete metadata collection
- **File Validation**: Size and type checking
- **Drag & Drop**: Modern file upload interface
- **Progress Tracking**: Loading states and feedback

### Dashboard
- **Statistics Cards**: Upload counts, downloads, points
- **Recent Activity**: User's latest actions
- **Quick Actions**: Fast access to key features
- **Responsive Layout**: Mobile-friendly design

### Firebase Integration
- **Authentication**: Secure user login/signup
- **Storage**: File upload to Firebase Storage
- **Firestore**: Metadata storage with timestamps
- **Security Rules**: User-based access control

## 🎨 Design Features

### Modern UI Elements
- **Card-based Layout**: Clean, organized interface
- **Color-coded Icons**: Visual subject categorization
- **Smooth Animations**: Hover effects and transitions
- **Typography**: Poppins font for readability

### Dark Mode Support
- **Theme Toggle**: Easy switching between themes
- **Consistent Styling**: All components support dark mode
- **Persistent Settings**: Theme preference saved locally

## 🔒 Security Features

### File Validation
- **Size Limits**: 10MB maximum file size
- **Type Restrictions**: Only PDF, JPG, PNG allowed
- **Content Validation**: Server-side verification

### User Authentication
- **Email/Password**: Secure login system
- **Session Management**: Persistent login states
- **Access Control**: User-specific uploads

## 📊 Data Structure

### Firestore Collections
```javascript
// PYQs Collection
{
  title: string,
  description: string,
  college: string,
  course: string,
  subject: string,
  year: number,
  semester: number,
  examType: string,
  fileName: string,
  fileSize: number,
  fileType: string,
  downloadURL: string,
  storageRef: string,
  uploadedBy: string,
  uploadedByEmail: string,
  uploadDate: timestamp,
  downloads: number,
  likes: number,
  status: string // pending, approved, rejected
}
```

## 🚀 Future Enhancements

### Planned Features
- **AI OCR**: Automatic text extraction from images
- **Advanced Search**: Filters and sorting options
- **Community Features**: Comments and ratings
- **Mobile App**: Native mobile application
- **Admin Panel**: Content moderation tools

### Technical Improvements
- **Performance**: Image optimization and caching
- **Security**: Enhanced file scanning
- **Analytics**: Usage tracking and insights
- **API**: RESTful API for third-party integration

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🆘 Support

For support or questions, please contact the development team or create an issue in the repository.

---

**Made with ❤️ by Team PYQ** 