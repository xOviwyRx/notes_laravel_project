# 📝 Laravel Notes Manager

[View Screenshot](../public/images/screenshots/screenshot.png)

A full-featured note-taking application with user authentication, built with Laravel and Docker.

## 🌟 Features

### ✅ Implemented
- **User Authentication**
    - Registration/login with [Laravel Breeze](https://laravel.com/docs/starter-kits)
    - Email verification
    - Password reset

- **Note Management**
    - Create, view, and edit notes
    - Rich text formatting
    - User-specific note isolation
    - Soft delete (trash system)

- **Technical Highlights**
    - RESTful Resource Controllers
    - Eloquent ORM with relationships
    - Database migrations
    - Dockerized environment

### 🚧 In Progress
- Permanent delete functionality
- Note categories/tags
- Search functionality

## 🛠 Tech Stack

| Category       | Technologies |
|----------------|--------------|
| **Backend**    | Laravel 10, PHP 8.2 |
| **Frontend**   | Blade, Tailwind CSS |
| **Database**   | MySQL 8 |
| **DevOps**     | Docker, Nginx |
| **Tools**      | Composer, Vite |

## 🚀 Installation

```bash
# Clone repository
git clone https://github.com/xOviwyRx/notes_laravel_project.git
cd notes_laravel_project

# Start containers
docker-compose up -d

# Install dependencies
docker-compose exec app composer install
docker-compose exec app npm install

# Setup environment
cp .env.example .env
docker-compose exec app php artisan key:generate
docker-compose exec app php artisan migrate

Access the app: http://localhost:8000
