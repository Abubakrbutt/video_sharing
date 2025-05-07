# Slide 0: Photo Sharing Platform
## A Scalable Cloud-Native Web Application
Student Name: [Your Name]
Student Number: [Your Student Number]

---

# Slide 1: The Problem
- Social media users want to share photos with others
- Users need different roles: creators (who upload) and consumers (who view)
- Traditional web hosting not suitable for growing user bases
- Need scalable solution for storing and serving media files
- Must handle multiple users accessing content at the same time

---

# Slide 2: Scalability Challenges
- Managing user authentication and different user roles
- Storing and retrieving large media files efficiently
- Database performance as content grows
- Handling high traffic during peak usage
- Resource optimization to minimize costs

---

# Slide 3: Technical Solution Overview
- Django web framework for backend development
- REST API for frontend-backend communication
- MySQL database for structured data storage
- Azure Blob Storage for media files
- Azure App Service for hosting web application

---

# Slide 4: Architecture Design
- Three-tier architecture:
  - Frontend (HTML/CSS/JS)
  - Backend (Django REST API)
  - Database (MySQL)
- Azure services integration
- Role-based access control
- Responsive design for different devices

---

# Slide 5: Core Features
- User authentication with distinct roles (creator/consumer)
- Media upload with metadata (title, caption, location, people)
- Search functionality by title, caption, or location
- Comment and rating system for consumers
- REST API for potential mobile app integration

---

# Slide 6: Database Design
- Custom User model with role-based permissions
- MediaContent model for storing uploaded media
- Comment and Rating models for user interactions
- Relationships between models for data integrity
- Pagination for efficient data retrieval

---

# Slide 7: Advanced Features
- RESTful API with token authentication
- Custom permissions based on user roles
- Media content search functionality
- Rating system with average score calculation
- Pagination for better performance with large datasets

---

# Slide 8: Caching and Performance
- Static files served from Azure CDN
- Database query optimization
- Image size optimization for faster loading
- API response caching
- Efficient database indexing

---

# Slide 9: Scalability Features
- Azure App Service with auto-scaling capability
- Azure MySQL Flexible Server for database scaling
- Stateless application design for horizontal scaling
- Optimized database queries to reduce load
- Pagination to handle large amounts of data

---

# Slide 10: Limitations and Future Improvements
- Current hosting plan has bandwidth limitations
- Need CDN integration for better global performance
- Better media processing for different formats
- Mobile app development
- Implementing real-time notifications

---

# Slide 11: Demo Video (5 minutes)
[The 5-minute demo video showcases the application functionality and Azure deployment, including:]
- Application overview and features
- User registration and role-based access
- Creator uploading photos with metadata
- Consumer viewing, searching, commenting on photos
- Azure deployment process and configuration
- Backend systems showing the application in action

---

# Slide 12: Conclusion
- Successfully implemented scalable photo sharing platform
- Met all core requirements using cloud-native approach
- Used Azure services for deployment and scaling
- Implemented role-based user management
- Created RESTful API for potential future extensions
- Deployed solution that can scale with growing user base

---

# Slide 13: References
- Django Documentation: https://docs.djangoproject.com/
- Django REST Framework: https://www.django-rest-framework.org/
- Azure App Service Documentation: https://learn.microsoft.com/en-us/azure/app-service/
- Azure MySQL Flexible Server: https://learn.microsoft.com/en-us/azure/mysql/flexible-server/
- Microsoft Learn - Deploy a Python web app: https://learn.microsoft.com/en-us/azure/app-service/quickstart-python
