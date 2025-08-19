# Django Commands Cheat Sheet

## 🔧 Project Setup
```bash
django-admin startproject projectname
python manage.py startapp appname
```

## ⚙️ Database
```bash
python manage.py makemigrations            # Create migration files
python manage.py migrate                   # Apply migrations to database
python manage.py sqlmigrate <app> <id>     # Show SQL for a migration
python manage.py showmigrations            # List migrations
```

## 🛠 Development
```bash
python manage.py runserver                 # Start dev server (default: 127.0.0.1:8000)
python manage.py runserver 0.0.0.0:8000    # Expose to all interfaces
python manage.py shell                     # Open Python shell with Django context
python manage.py check                     # Check project for errors
python manage.py test                      # Run tests
```

## 👤 Users & Auth
```bash
python manage.py createsuperuser           # Create admin user
python manage.py changepassword <username> # Change user password
```

## 📦 Apps & Management
```bash
python manage.py listapps                  # List installed apps (Django 3.2+)
python manage.py dumpdata > data.json      # Export data to JSON
python manage.py loaddata data.json        # Import data from JSON
```

## 🔍 Debugging / Utilities
```bash
python manage.py showurls                  # Show all project URLs (requires django-extensions)
python manage.py dbshell                   # Open database shell
python manage.py diffsettings              # Show settings differences from defaults
```