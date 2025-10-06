# 🏆 CodeQuest - Elevate Your Coding Skills

[![Django](https://img.shields.io/badge/Django-5.0.7-green.svg)](https://www.djangoproject.com/)
[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-2.2.19-38B2AC.svg)](https://tailwindcss.com/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

**CodeQuest** is a modern, feature-rich competitive programming platform designed to help developers master algorithmic problem-solving skills. Built with Django and enhanced with a beautiful gradient UI, CodeQuest provides an engaging environment for learning, practicing, and excelling in coding challenges.

> 🚀 **Challenge yourself, track your progress, and become a coding champion!**

## ✨ Features

### 🎯 Core Functionality

- **🏠 Smart Dashboard**: Intuitive problem browser with advanced filtering by difficulty, tags, and search terms
- **💻 Professional Code Editor**: CodeMirror-powered editor with syntax highlighting and Python support
- **⚡ Real-time Code Execution**: Fast code evaluation using Judge0 API (< 3 seconds response time)
- **📊 Comprehensive Analytics**: Detailed submission history and performance tracking
- **🏷️ Tag-based Organization**: Problems categorized by topics like arrays, graphs, dynamic programming

### 👤 User Experience

- **🔐 Secure Authentication**: Custom user management with secure login/registration
- **📈 Progress Tracking**: Visual progress bars and statistics by difficulty level
- **🎨 Modern UI/UX**: Beautiful gradient design with glass-morphism effects
- **📱 Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **🌟 Interactive Elements**: Smooth animations, hover effects, and transitions

### 🔧 Technical Features

- **🎨 Glass-morphism Design**: Modern UI with backdrop blur effects and gradient backgrounds
- **🔍 Advanced Search**: Multi-parameter filtering (title, description, difficulty, tags)
- **📄 Pagination**: Efficient handling of large problem sets
- **🎪 Interactive Tabs**: Seamless navigation between problem, editorial, and submissions
- **💾 Session Management**: Persistent user sessions and data

## 🛠️ Technologies Used

### Backend Stack

- **🐍 Django 5.0.7**: Modern Python web framework
- **🔌 Django REST Framework**: API development and serialization
- **🗄️ SQLite**: Lightweight database for development
- **🔒 Python Decouple**: Environment variable management

### Frontend Stack

- **🎨 Tailwind CSS 2.2.19**: Utility-first CSS framework
- **💻 CodeMirror 5.65.5**: Professional code editor
- **⚡ Vanilla JavaScript**: Interactive functionality and AJAX calls
- **🎭 Custom CSS**: Animations, gradients, and glass-morphism effects

### External Services

- **⚖️ Judge0 API**: Code compilation and execution
- **🌐 Font Awesome**: Icon library (optional)

## 🚀 Quick Start

### Prerequisites

- Python 3.8+
- pip (Python package manager)
- Git

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/srikaran3004/Code-Quest.git
   cd Code-Quest
   ```

2. **Create and activate virtual environment**

   ```bash
   # Windows
   python -m venv venv
   venv\Scripts\activate

   # macOS/Linux
   python3 -m venv venv
   source venv/bin/activate
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Environment Configuration**
   Create a `.env` file in the root directory:

   ```env
   SECRET_KEY=your-super-secret-key-here
   DEBUG=True
   ALLOWED_HOSTS=localhost,127.0.0.1
   ```

5. **Database Setup**

   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

6. **Create Superuser (Optional)**

   ```bash
   python manage.py createsuperuser
   ```

7. **Run the Development Server**

   ```bash
   python manage.py runserver
   ```

8. **Access the Application**
   Open your browser and navigate to `http://127.0.0.1:8000`

## 📁 Project Structure

```
CodeQuest/
├── 📁 CodeQuest/          # Main project configuration
│   ├── settings.py        # Django settings
│   ├── urls.py           # URL routing
│   └── wsgi.py           # WSGI configuration
├── 📁 custom_auth/        # User authentication app
│   ├── models.py         # Custom user model
│   ├── views.py          # Auth views
│   └── templates/        # Auth templates
├── 📁 Quest/              # Core problem-solving app
│   ├── models.py         # Problem, TestCase, Submission models
│   ├── views.py          # Problem views and logic
│   └── templates/        # Problem templates
├── 📁 user_profile/       # User profile management
├── 📁 api/                # REST API endpoints
├── 📁 static/             # Static files (CSS, JS, images)
└── 📁 templates/          # Shared templates
```

## 🎮 How to Use

### For Students/Learners

1. **📝 Register**: Create your account to start your coding journey
2. **🔍 Explore**: Browse problems by difficulty or search by topic
3. **💻 Code**: Use the integrated editor to write your solutions
4. **🧪 Test**: Run your code against test cases instantly
5. **📊 Track**: Monitor your progress and improvement over time

### For Educators

1. **➕ Add Problems**: Use the admin panel to create new coding challenges
2. **🏷️ Organize**: Tag problems by topic for better organization
3. **📈 Monitor**: Track student progress and identify learning gaps
4. **✏️ Customize**: Modify test cases and problem descriptions

## 🎨 UI/UX Enhancements (2025 Update)

### Design Improvements

- **🌈 Modern Gradient Theme**: Shifted from purple to blue-green gradients
- **🔮 Glass-morphism Effects**: Translucent cards with backdrop blur
- **✨ Enhanced Animations**: Smooth transitions and hover effects
- **📱 Mobile-First Design**: Responsive layout for all screen sizes

### New Features

- **🎯 Welcome Dashboard**: Personalized greeting with progress overview
- **🏆 Achievement System**: Visual progress indicators and stats
- **🎪 Interactive Filter UI**: Enhanced tag selection with visual feedback
- **📊 Improved Analytics**: Better progress visualization and success rates

### User Experience

- **⚡ Faster Navigation**: Streamlined user flows and reduced clicks
- **🎨 Consistent Branding**: Unified color scheme and typography
- **🔍 Better Search**: Enhanced filtering with visual indicators
- **📈 Progress Visualization**: Beautiful progress bars and statistics

## 🤝 Contributing

I welcome contributions from the community! Here's how you can help:

### Development Setup

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Make your changes and test thoroughly
4. Commit with clear messages: `git commit -m "Add feature description"`
5. Push to your fork: `git push origin feature-name`
6. Create a Pull Request

### Contribution Guidelines

- Follow Django best practices and PEP 8 style guide
- Write clear, concise commit messages
- Include tests for new features
- Update documentation as needed
- Ensure responsive design compatibility

## 🔧 API Documentation

### Authentication Endpoints

- `POST /auth/login/` - User login
- `POST /auth/register/` - User registration
- `POST /auth/logout/` - User logout

### Problem Endpoints

- `GET /api/problems/` - List all problems
- `GET /api/problems/{id}/` - Get specific problem
- `POST /api/problems/{id}/submit_solution/` - Submit solution
- `GET /api/problems/{id}/submissions/{user_id}/` - Get user submissions

## 🐛 Troubleshooting

### Common Issues

**1. Virtual Environment Issues**

```bash
# Recreate virtual environment
rm -rf venv
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
pip install -r requirements.txt
```

**2. Database Migration Errors**

```bash
# Reset migrations
python manage.py migrate --fake-initial
python manage.py makemigrations
python manage.py migrate
```

**3. Static Files Not Loading**

```bash
# Collect static files
python manage.py collectstatic
```

## 📈 Future Roadmap

### Planned Features

- **🏆 Leaderboards**: Global and category-specific rankings
- **👥 Team Competitions**: Collaborative problem-solving events
- **🧠 AI Hints**: Smart hints and solution explanations
- **📚 Learning Paths**: Structured curriculum for different topics
- **🔔 Notifications**: Real-time updates and reminders
- **📊 Advanced Analytics**: Detailed performance insights
- **🌐 Multi-language Support**: Support for multiple programming languages
- **💾 Cloud Synchronization**: Cross-device progress sync

### Technical Improvements

- **🚀 Performance Optimization**: Faster loading and better caching
- **🔐 Enhanced Security**: Advanced authentication and authorization
- **📱 Mobile App**: Native iOS and Android applications
- **☁️ Cloud Deployment**: Production-ready hosting solution

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Django Community**: For the excellent web framework
- **Judge0**: For providing reliable code execution services
- **Tailwind CSS**: For the utility-first CSS framework
- **CodeMirror**: For the professional code editor
- **Community Contributors**: For their valuable feedback and contributions

<div align="center">

**🚀 Ready to start your coding journey?**

[**Launch CodeQuest**](http://127.0.0.1:8000) | [**Report Bug**](https://github.com/yourusername/Code-Quest/issues) | [**Request Feature**](https://github.com/srikaran3004/Code-Quest/issues)

Made with ❤️ by the Srikaran

</div>
