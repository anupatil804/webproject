🛍️ ShopEasy — React E-Commerce Website

ShopEasy is a modern **React-based e-commerce web application** designed to provide users with a simple and interactive online shopping experience.

The application includes product browsing, user registration and login, shopping cart functionality, product purchasing, feedback, and Firebase integration for authentication and data storage.

---

 Live Project

GitHub Repository:
https://github.com/anupatil804/webproject

---

 About the Project

ShopEasy is developed using **React.js** and provides a user-friendly interface for browsing and purchasing products online.

The project was created to practice and demonstrate important front-end development concepts such as:

* React components
* React Router
* CSS styling
* Form handling
* State management
* Firebase Authentication
* Firebase Realtime Database
* Product management
* Shopping cart functionality
* Responsive web design

---

 Features

 Home Page

* Attractive homepage
* Navigation menu
* Product-related content
* Easy access to different sections

 User Registration

* New users can create an account
* Registration form
* Firebase Authentication integration

 User Login

* Existing users can log in
* Firebase Authentication
* Login validation

 Products

* Displays available products
* Product images
* Product names
* Product prices
* Product details
* Buy Now functionality

 Shopping Cart

* Add products to cart
* View selected products
* Manage cart items
* Calculate product totals

 Buy Now

* Purchase interface
* Selected product information
* Order-related functionality

 Feedback

* Users can submit feedback
* Feedback page for customer interaction

 About Page

* Information about ShopEasy
* Project/company information

 Firebase Integration

The application uses Firebase for:

* User authentication
* User registration
* User login
* Realtime Database
* Product-related data

---

Technologies Used

| Technology                     | Purpose                     |
| ------------------------------ | --------------------------- |
| **React.js**                   | Front-end development       |
| **JavaScript**                 | Application logic           |
| **HTML5**                      | Page structure              |
| **CSS3**                       | Styling and layout          |
| **React Router DOM**           | Page navigation             |
| **Firebase Authentication**    | User registration and login |
| **Firebase Realtime Database** | Data storage                |
| **Git**                        | Version control             |
| **GitHub**                     | Source code hosting         |
| **npm**                        | Package management          |

---

 Project Structure

```text
webproject/
│
├── public/
│   ├── favicon.ico
│   ├── index.html
│   ├── logo192.png
│   ├── logo512.png
│   ├── manifest.json
│   └── robots.txt
│
├── src/
│   │
│   ├── assets/
│   │   ├── about.jpg
│   │   ├── back.jpg
│   │   ├── earphone.jpg
│   │   ├── feedback.jpg
│   │   ├── image.jpg
│   │   ├── imagee.jpg
│   │   ├── product1.jpg
│   │   ├── product2.jpg
│   │   ├── product3.jpg
│   │   ├── product4.jpg
│   │   ├── product5.jpg
│   │   ├── product6.jpg
│   │   ├── product7.jpg
│   │   ├── product8.jpg
│   │   └── registration.jpg
│   │
│   ├── component/
│   │   ├── About.js
│   │   ├── About.css
│   │   ├── BuyNow.js
│   │   ├── BuyNow.css
│   │   ├── Cart.js
│   │   ├── Cart.css
│   │   ├── Feedback.js
│   │   ├── Feedback.css
│   │   ├── Home.js
│   │   ├── Home.css
│   │   ├── Login.js
│   │   ├── Login.css
│   │   ├── Navbar.js
│   │   ├── Navbar.css
│   │   ├── Product.js
│   │   ├── Product.css
│   │   ├── Registration.js
│   │   └── Registration.css
│   │
│   ├── App.js
│   ├── App.css
│   ├── firebase.js
│   ├── index.js
│   ├── index.css
│   └── ...
│
├── .gitignore
├── package.json
├── package-lock.json
└── README.md
```

---

 Application Routes

ShopEasy uses **React Router DOM** for navigation.

| Route           | Page          |
| --------------- | ------------- |
| `/`             | Home          |
| `/about`        | About         |
| `/login`        | Login         |
| `/registration` | Registration  |
| `/Product`      | Products      |
| `/Feedback`     | Feedback      |
| `/BuyNow`       | Buy Now       |
| `/Cart`         | Shopping Cart |

---

 Sample Products

The project includes several sample products.

| Product     | Example Price |
| ----------- | ------------: |
| Smart Watch |        ₹1,999 |
| Headphones  |        ₹1,499 |
| Shoes       |        ₹2,499 |
| Product 4   |             — |
| Product 5   |             — |
| Product 6   |             — |
| Product 7   |             — |
| Product 8   |             — |

Product information can be managed through the Firebase Realtime Database.

---

Getting Started

Follow the steps below to run ShopEasy on your local computer.

 Clone the Repository

Open Command Prompt or Terminal and run:


git clone https://github.com/anupatil804/webproject.git




 2. Open the Project

```bash
cd webproject
```

---

 3. Install Dependencies

Run:


npm install


If your Windows environment has an issue with `npm.ps1`, you can use:


npm.cmd install



 4. Configure Firebase

The project uses Firebase for authentication and database functionality.

Open:


src/firebase.js


Add your own Firebase project configuration.

Example:

```javascript
import { initializeApp } from "firebase/app";
import { getAuth } from "firebase/auth";
import { getDatabase } from "firebase/database";

const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_AUTH_DOMAIN",
  databaseURL: "YOUR_DATABASE_URL",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_STORAGE_BUCKET",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID"
};

const app = initializeApp(firebaseConfig);

export const auth = getAuth(app);
export const db = getDatabase(app);
```

> ⚠️ **Security Note:** Do not upload private credentials, passwords, service-account JSON files, or other sensitive secrets to GitHub.

---

## 5. Start the Development Server

Run:

```bash
npm start
```

Or, if required on Windows:


npm.cmd start


The application will normally open at:


http://localhost:3000




 Firebase Setup

To use the authentication and database features:

Step 1 — Create a Firebase Project

Go to the Firebase Console and create a new project.

 Step 2 — Add a Web App

Create a web application inside your Firebase project.

Step 3 — Enable Authentication

Enable the authentication methods required by the application, such as:

* Email/Password

Step 4 — Create Realtime Database

Create a Firebase Realtime Database.

The project uses the database for application data such as products and user-related information.

---
 Main React Components

`Navbar`

Provides navigation between different pages.

 `Home`

Displays the main ShopEasy landing page.

 `About`

Provides information about the project.

 `Product`

Displays available products and shopping options.

 `Login`

Allows existing users to authenticate.

 `Registration`

Allows new users to create an account.

 `Cart`

Displays products selected by the user.

 `BuyNow`

Handles the product purchase interface.

 `Feedback`

Allows users to submit feedback.

---

 Responsive Design

The application uses CSS to create a user-friendly interface across different screen sizes.

The design can be further improved for:

* Desktop
* Laptop
* Tablet
* Mobile devices


 Git Workflow

After making changes to the project, use:


git add .
git commit -m "Updated project"
git push


For example:


git add .
git commit -m "Added new product feature"
git push


This will upload your latest changes to GitHub.



 Available Scripts

Inside the project directory, you can run:

 Start Development Server

bash
npm start


 Run Tests


npm test


 Create Production Build


npm run build

Eject Configuration


npm run eject


> **Note:** `npm run eject` is generally irreversible, so use it only when you understand why you need it.

---

 Future Improvements

Some possible future improvements include:

* 💳 Online payment integration
* 📦 Order tracking
* ❤️ Wishlist functionality
* 🔎 Product search
* 🏷️ Product categories and filters
* ⭐ Product ratings and reviews
* 👤 User profile page
* 📋 Order history
* 🛒 Improved cart management
* 📱 Improved mobile responsiveness
* 🔔 Order notifications
* 🧑‍💼 Admin dashboard
* 📊 Admin product management

---

  Learning Objectives

This project demonstrates practical usage of:

* React components
* Props and state
* React hooks
* React Router
* Forms
* Event handling
* CSS
* Firebase Authentication
* Firebase Realtime Database
* CRUD-related operations
* Git and GitHub

---

  Developer

Anushka Patil**

BCA Graduate & Aspiring Software Professional

---

  License

This project is created for **educational and portfolio purposes**.

You are welcome to study and modify the project for learning purposes.

---

 Acknowledgement

This project was developed as a learning project to practice modern front-end web development using **React.js and Firebase**.

If you find the project useful, consider giving the repository a ⭐ on GitHub.



 📌 Repository

**ShopEasy — React E-Commerce Website**

https://github.com/anupatil804/webproject
