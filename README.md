# CityLife — Angular Frontend Application

🌐 **Live Demo**  
https://citylife1.netlify.app/

CityLife is a **frontend-only web application built with Angular**, designed to simulate a small social platform.
The application integrates with the **GoRest public REST API** to handle users, posts, and comments through real-world CRUD operations.

This project is part of my portfolio and focuses on **modern Angular development**, API integration, and responsive UI design.

---

## Overview

CityLife allows authenticated users to:

- Log in using an external API token
- Browse, create, and delete users
- View user profiles
- Create, filter, and manage posts
- Add and delete comments
- Switch between English and Italian

The UI is fully responsive and optimized for both **desktop and mobile devices**.

---

## Authentication

Authentication is handled via the **GoRest API**.

To access the application:
1. Obtain an API token from: https://gorest.co.in/consumer/login
2. Use the token in the login form

The token is required to access protected routes and perform write operations.

---

## Users Management

The Users page provides full user management features:

- View all users
- Search users by name or email
- Create new users
- Delete existing users
- Visual status indicator:
  - 🟢 Active
  - 🔴 Inactive
- Pagination and dynamic page-size selection

---

## User Profile

Each user has a dedicated profile page containing:

- Personal details (name, email, status)
- A list of published posts
- Ability to:
  - Create new posts
  - View comments
  - Add comments
  - Delete posts and comments

If a user has no posts, the following fallback message is displayed:
```
No posts available
```

---

## Posts & Comments

The Posts section allows users to:

- View a global posts feed
- Create new posts
- Delete posts
- Filter posts by text
- Navigate posts using pagination
- Select the number of posts per page
- Manage comments (view, add, delete)

---

## Internationalization

CityLife supports **English and Italian**.

- Language can be selected on the login page
- It can be changed at any time using the navbar toggle

---

## Logout

A logout action is available in the navigation bar.
Logging out clears the session and redirects the user to the login page.

---

## Tech Stack

- **Angular**
- **TypeScript**
- **HTML5**
- **SCSS**
- **Angular CLI**
- **GoRest REST API**
- **Netlify** (deployment)

---

## Getting Started

### Prerequisites

- Node.js
- Angular CLI

### Installation

```bash
git clone https://github.com/Aldosimone99/CityLife.git
cd CityLife
npm install
```

### Run locally

```bash
ng serve
```

Open your browser at:
http://localhost:4200

---

## API Integration

This project consumes the **GoRest REST API**.

### Users
- `GET /v2/users`
- `POST /v2/users`
- `PUT /v2/users/:userId`
- `DELETE /v2/users/:userId`

### Posts
- `GET /v2/posts`
- `GET /v2/users/:userId/posts`
- `POST /v2/users/:userId/posts`

### Comments
- `GET /v2/posts/:postId/comments`
- `POST /v2/posts/:postId/comments`

---

## Purpose of the Project

This project was created to:

- Practice **Angular frontend architecture**
- Work with a real external REST API
- Implement authentication and CRUD flows
- Build a responsive, production-like UI
- Serve as a **portfolio project** for frontend and full-stack roles

---

## Author

**Aldosimone Di Rosa**  
Frontend Developer (React) · Full-Stack aware  
📍 Italy · 🌍 Open to US Remote

- Portfolio: https://aldosimone99.github.io
- GitHub: https://github.com/Aldosimone99
- LinkedIn: https://www.linkedin.com/in/aldosimone-di-rosa-b5a55716b/

---

## License

This project is intended for educational and portfolio purposes.
