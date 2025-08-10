
---

##  Key Features

- **Custom User** model with additional phone number field.
- **Post Management**: Users can create, update, and delete blog posts with optional image uploads.
- **Categorization**: Posts are classified by categories such as Python, Java, JavaScript, C++, MySQL, or Others.
- **Interactions**: 
  - Users can **like** and **comment** on posts.
  - Supports a **follow request system** — users can send, accept, or remove follow requests.
- **Views**:
  - **World View**: Display all posts to all users.
  - **Personal View**: View your own posts, friends’ posts, and manage follow requests.
  - **Search**: Search posts by title with live result listing.
  - **Post Detail**: Like/unlike, comment, and manage posts (if author or admin).
- **Tailwind Theme** integration via the `theme` app for styling.

---

##  Tech Stack

- **Backend**: Django (version 5.x) with custom authentication.
- **Templating**: Django Templates
- **Styling**: Tailwind CSS via integrated `theme` app
- **Database**: SQLite (default)
- **Static & Media**: Handled by Django’s settings (`static/` and `media/` directories)

---

##  Installation & Setup

```bash
# 1. Clone the repository
git clone https://github.com/your-username/bloggyweb.git
cd bloggyweb

# 2. Create and activate a virtual environment
python -m venv venv
source venv/bin/activate  # or `venv\Scripts\activate` on Windows

# 3. Install dependencies
pip install -r requirments.txt

# 4. Apply migrations
python manage.py migrate

# 5. Create a superuser (optional, for admin access)
python manage.py createsuperuser

# 6. Run the development server
python manage.py runserver
