---

**What Was Implemented This Week**

This week, the team set up the frontend folder in the GitHub repository and built the HTML pages based on the use case diagram. All pages were styled with Bootstrap 5, and placeholders were prepared for the API connection. The updated /frontend folder was pushed to GitHub, with screenshots of the pages added in /docs/lab11.

frontend/

├── index.html

├── login.html

├── register.html

├── dashboard.html

├── profile.html

├── css/

├── js/

└── img/

---

**Alignment with the Use Case Diagram**

Log in is handled by login.html and Update Profile Info by profile.html, both shared by the user and admin. The user-only use cases, Post, Comment, and React, are handled on dashboard.html. Although register.html is not in the diagram, it supports the Log in flow by allowing new users to be created. The admin-only use cases, Manage user accounts and Review reports, are planned for a later week.

---

**Alignment with the ERD**

The pages follow the four ERD collections. The User fields (username, email, password) appear in the register, login, and profile pages. Post fields (title, content, author, createdAt) appear in the dashboard's create-post form and post cards. Comment fields (text, author, post) appear as a comment input and list under each post. The Like collection supports the React use case through a like button and count on each post. Foreign keys such as author, post, and user determine how the interface links items together, for example showing each author's name and grouping comments under their post.

---

**Planned Change: React Use Case**

The React use case is under review and may be simplified or removed in a future iteration to keep the project scope manageable. A final decision is pending.

---

**The following components are tied to this use case and may be revised accordingly:**

-Use Case Diagram – the React use case for users

-ERD – the Like collection

-API placeholders – POST /posts/:id/likes

---

**API Connection Placeholders**

Placeholders in the /js folder are tied to each collection: POST /auth/register and POST /auth/login for User, GET/POST /posts for Post, GET/POST /posts/:id/comments for Comment, and POST /posts/:id/likes for Like. These paths may change once the backend routes are finalized.

---

**Tools Used**

-HTML5

-CSS 

-JavaScript 

-Bootstrap 5 

-Git and GitHub

-MongoDB

