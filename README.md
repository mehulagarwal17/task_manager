# 📋 TaskMaster - Modern Task Management App

A sleek, modern Django-based task management application with a beautiful UI featuring a black and pink color scheme. Built with Django 4.2.7 and deployed on Render.

Deployed Link : https://taskmanager-m40n.onrender.com

## ✨ Features

### 🎨 Modern UI/UX
- **Stunning Design**: Black background with vibrant pink accents
- **Responsive Layout**: Works perfectly on all devices
- **Cylindrical Navigation**: Transparent navbar with modern styling
- **Smooth Animations**: Hover effects and transitions throughout
- **Typography**: Modern Poppins font for professional appearance

### 🔐 User Authentication
- **Secure Registration**: User signup with validation
- **Login System**: Secure authentication with Django's built-in User model
- **Session Management**: Persistent login sessions
- **Password Security**: Encrypted password storage

### 📝 Task Management
- **Create Tasks**: Add new tasks with title and description
- **Edit Tasks**: Update existing task details
- **Delete Tasks**: Remove completed or unwanted tasks
- **Task Status**: Mark tasks as completed or pending
- **User-Specific Tasks**: Each user sees only their own tasks

### 🌟 Landing Page
- **Hero Section**: Eye-catching introduction with modern design
- **Features Showcase**: Highlight key app capabilities
- **Statistics Display**: Impressive metrics and achievements
- **Call-to-Action**: Clear user engagement prompts
- **Professional Footer**: Complete with links and information

## 🚀 Live Demo

🌐 **Deployed on Render**: [TaskMaster Live](https://taskmanager-m40n.onrender.com)

## 🛠️ Technology Stack

### Backend
- **Django 4.2.7**: Python web framework
- **SQLite3**: Database for development
- **Gunicorn**: Production web server
- **WhiteNoise**: Static file serving

### Frontend
- **HTML5**: Semantic markup
- **CSS3**: Modern styling with animations
- **Responsive Design**: Mobile-first approach
- **Google Fonts**: Poppins typography

### Deployment
- **Render**: Cloud hosting platform
- **GitHub**: Version control and CI/CD
- **Procfile**: Deployment configuration

## 📦 Installation & Setup

### Prerequisites
- Python 3.8+
- Git
- Virtual environment (recommended)

### Local Development Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/mehulagarwal17/task_manager.git
   cd task_manager
   ```

2. **Create virtual environment**
   ```bash
   python -m venv venv
   
   # Windows
   venv\Scripts\activate
   
   # Mac/Linux
   source venv/bin/activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run migrations**
   ```bash
   python manage.py migrate
   ```

5. **Create superuser (optional)**
   ```bash
   python manage.py createsuperuser
   ```

6. **Run development server**
   ```bash
   python manage.py runserver
   ```

7. **Access the application**
   - Open: `http://127.0.0.1:8000`
   - Admin: `http://127.0.0.1:8000/admin`

## 🎯 Project Structure

```
task_manager/
├── taskmanagement/          # Django project settings
│   ├── __init__.py
│   ├── settings.py         # Main configuration
│   ├── urls.py            # URL routing
│   └── wsgi.py            # WSGI configuration
├── task/                   # Django app
│   ├── migrations/        # Database migrations
│   ├── templates/         # HTML templates
│   ├── admin.py          # Admin configuration
│   ├── forms.py          # Django forms
│   ├── models.py         # Database models
│   ├── urls.py           # App URLs
│   └── views.py          # View functions
├── static/                # Static files (CSS, JS, images)
│   └── styles.css        # Main stylesheet
├── templates/             # Base templates
├── db.sqlite3           # SQLite database
├── manage.py            # Django management script
├── requirements.txt     # Python dependencies
├── Procfile            # Render deployment config
└── README.md           # This file
```

## 🎨 Design System

### Color Palette
- **Black**: `#000000` - Primary background
- **Dark Pink**: `#C2185B` - Secondary accents
- **Bright Pink**: `#E91E63` - Primary accent color
- **Light Pink**: `#F8BBD0` - Subtle highlights
- **White**: `#FFFFFF` - Text and primary content

### Typography
- **Font Family**: Poppins (Google Fonts)
- **Weights**: 300 (Light), 400 (Regular), 500 (Medium), 600 (Semi-Bold), 700 (Bold)

### UI Components
- **Cards**: Glassmorphism effect with backdrop blur
- **Buttons**: Gradient backgrounds with hover animations
- **Navigation**: Cylindrical transparent design
- **Forms**: Modern input styling with focus states

## 🚀 Deployment Guide

### Render Deployment

1. **Prepare for Production**
   - Update `ALLOWED_HOSTS` in settings.py
   - Set `DEBUG = False` in production
   - Configure environment variables

2. **Required Files**
   - `requirements.txt`: Python dependencies
   - `Procfile`: Deployment commands
   - Environment variables: `SECRET_KEY`, `DEBUG`

3. **Render Configuration**
   ```yaml
   Build Command: pip install -r requirements.txt && python manage.py collectstatic --noinput
   Start Command: gunicorn taskmanagement.wsgi:application --bind 0.0.0.0:$PORT
   Environment Variables:
     - DEBUG=False
     - SECRET_KEY=your-secret-key-here
   ```

4. **Deploy Steps**
   - Connect GitHub repository to Render
   - Configure web service settings
   - Add environment variables
   - Deploy and monitor logs

## 🔧 Configuration

### Environment Variables
- `DEBUG`: Set to `False` in production
- `SECRET_KEY`: Generate unique secret key
- `ALLOWED_HOSTS`: Add your domain name

### Database
- **Development**: SQLite3 (default)
- **Production**: Can be configured for PostgreSQL/MySQL

## 📱 Features in Detail

### User Authentication
- Registration with username and password
- Secure login/logout functionality
- Password validation and hashing
- Session-based authentication

### Task Management
- CRUD operations for tasks
- User-specific task isolation
- Task completion tracking
- Rich text descriptions

### UI/UX Highlights
- **Hero Section**: Modern landing with animated elements
- **Responsive Grid**: Adaptive layout for all screen sizes
- **Micro-interactions**: Hover states and transitions
- **Loading States**: Smooth user experience
- **Error Handling**: User-friendly error messages

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Django Team**: For the amazing web framework
- **Render**: For providing hosting services
- **Google Fonts**: For the Poppins font family
- **Community**: For inspiration and support

## 📞 Contact

- **GitHub**: [@mehulagarwal17](https://github.com/mehulagarwal17)
- **Live App**: [TaskMaster on Render](https://taskmanager-m40n.onrender.com)

---

⭐ **If you like this project, please give it a star!**

🚀 **Built with ❤️ using Django and deployed on Render**
