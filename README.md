# ChillPill

## Short Brief

"ChillPill: Your Stress-Relief Hub 🌿

- 🧘‍♀️ Relax with soothing music, yoga, and meditation videos.
- 🍲 Find recipes for any ingredient in our diet section.
- 📖 Create your personal diary and connect with others.
- 🔒 Secure login/sign-up for a personalized experience.
  Experience calm and connection at ChillPill!"

## Contents:

- About
- Project Starter
- Glimpse of the site
- Tools and Packages
- Author

---

# ✊ About

> ChillPill stresses on reducing people's stress and anxiety by providing featues like therapy, diet, diary and chat sections.

The deployed link is [ChillPill](https://chill-pill-two.vercel.app/)

---

# 👨‍💻 Getting started

This section will work you through how you can get started with the project.

### Directory Layout

<pre>
.
├── <strong>client</strong>
|      ├── <strong>public</strong>
|      └── <strong>src</strong>
|           ├── <strong>assets</strong>
|           |
|           ├── <strong>Components</strong>
|           │      ├── <strong>ChatComponents</strong>  
|           |      |        ├──<strong>ChatContainer.js</strong>
|           │      |        ├──<strong>ChatInput.js</strong>
|           │      |        ├──<strong>Contacts.js</strong>
|           │      |        └──<strong>Welcome.js</strong> 
|           |      ├── <strong>DiaryComponents</strong>  
|           │      |        └──<strong>DiaryEntry.js</strong> 
|           |      ├── <strong>DietComponents</strong>  
|           |      |        ├──<strong>DietLists.js</strong>
|           │      |        └──<strong>RecipeTile.js</strong> 
|           |      ├── <strong>HomeComponents</strong>  
|           |      |        ├──<strong>Button.js</strong>
|           │      |        └──<strong>Footer.js</strong>
|           |      ├── <strong>NavbarComponents</strong>  
|           |      |        ├──<strong>Logout.js</strong>
|           │      |        └──<strong>Navbar.js</strong>
|           │      └── <strong>TherapyComponents</strong>
|           │               └──<strong>Frames.js</strong>
|           │  
|           ├── <strong>Pages</strong>
|           │      ├── <strong>Chat.js</strong>
|           │      ├── <strong>Diary.js</strong>
|           │      ├── <strong>Diet.js</strong>
|           │      ├── <strong>Home.js</strong>
|           │      ├── <strong>Login.js</strong>
|           │      ├── <strong>Register.js</strong>
|           │      ├── <strong>SetAvatar.js</strong>
|           │      └── <strong>Therapy.js</strong> 
|           │ 
|           ├── <strong>Utils</strong>
|           │      └── <strong>APIRoutes.js</strong>     
|           │ 
|           ├── <strong>App.js</strong>
|           │ 
|           ├── <strong>index.css</strong>
|           │ 
|           └── <strong>index.js</strong>
|
│   
│ 
├── <strong>server</strong>
|      ├── <strong>Controllers</strong>
|      │      ├── <strong>diaryControllers.js</strong>
|      │      ├── <strong>messageControllers.js</strong>
|      │      └── <strong>userControllers.js</strong> 
|      │
|      ├── <strong>Model</strong>
|      │      ├── <strong>diaryModel.js</strong>
|      │      ├── <strong>messageModel.js</strong>
|      │      └── <strong>userModel.js</strong> 
|      │
|      ├── <strong>Routes</strong>
|      │      ├── <strong>diaryRoutes.js</strong>
|      │      ├── <strong>messageRoutes.js</strong>
|      │      └── <strong>userRoutes.js</strong> 
|      │  
|      └── index.js
|  
|
└── README.md
</pre>

### Run on your local server

You will need [NodeJS](), [Git]() and [MongoDB]() installed to run this project locally

      node@v16.13.0 or higher
      npm@8.1.0 or higher
      git@2.34.1 or higher

If you dont have [MongoDB]() you use [MongoDB Atls]()

1. Clone the repo

```bash
git clone https://github.com/aham-18113/ChillPill.git
```

2. Create a file called .env in the Backend directory of your project:

   server
   └──- Controllers - Model - Routes - .env <-- create it here - .gitignore - index.js - package-lock.json - package.json

3. Inside the .env file, add key `MONGO_URL` and assign your MongoDB local host or Mongo Atls like this

```bash
# .env
MONGO_URL = "YOUR_DB_LOCAL_HOST"
```

1. Starting the Server application.

```bash
cd server
npm install
nodemon index.js
```

`This will start server on localhost:5000`

5. Starting the Client application.

```bash
cd client
npm install
npm start
```

`This will start client app on localhost:3000`

---

# 🧰 Tools & Packages

## Client Dependencies

| Package                                                                | Description                                                                    | version |
| ---------------------------------------------------------------------- | ------------------------------------------------------------------------------ | ------- |
| [axios](https://www.npmjs.com/package/axios)                           | Promise based HTTP client for the browser and node.js                          | 0.27.2  |
| [buffer](https://www.npmjs.com/package/buffer)                         | A package for easy manipulation of binary data                                 | 6.0.3   |
| [emoji-picker-react](https://www.npmjs.com/package/emoji-picker-react) | To add Emoji picker component for react applications                           | 3.5.1   |
| [material-ui-icons](https://mui.com/material-ui/material-icons/)       | Ready-to-use React Material Icons from the mui library                         | 5.8.4   |
| [react-icons](https://react-icons.github.io/react-icons)               | A library that allows us to include only those icons that our project is using | 4.4.0   |
| [react-toastify](https://www.npmjs.com/package/react-toastify)         | A package that allows to add notifications to our app with ease                | 9.0.5   |
| [socket.io-client](https://socket.io/docs/v4/client-api/)              | A package for client-side implementation of socket.io                          | 4.5.1   |
| [styled-components](https://styled-components.com/)                    | A library which lets you write CSS in your JavaScript                          | 5.3.5   |
| [uuid](https://www.npmjs.com/package/uuid)                             | A package used for identifying information that needs to be unique             | 8.3.2   |

## Server Dependencies

| Package                                        | Description                                                                  | version |
| ---------------------------------------------- | ---------------------------------------------------------------------------- | ------- |
| [bcrypt](https://www.npmjs.com/package/bcrypt) | A library to help you hash password                                          | 5.0.1   |
| [cors](https://www.npmjs.com/package/cors)     | A package providing express middleware                                       | 2.8.5   |
| [dotenv](https://www.npmjs.com/package/dotenv) | A library that loads environment variables from a .env file into process.env | 16.0.1  |
| [express](https://expressjs.com)               | Node.js web application framework for server side scripting                  | 4.18.1  |
| [MongoDB](https://www.mongodb.com)             | A NoSQL database                                                             | 4.4.3   |
| [mongoose](https://mongoosejs.com)             | Elegant mongodb object modeling for node.js                                  | 6.4.0   |
| [socket.io](https://socket.io/)                | A library enabling real-time bidirectional event-based communication         | 4.5.1   |

## Server devDependencies

| Package                                          | Description                                         | version |
| ------------------------------------------------ | --------------------------------------------------- | ------- |
| [nodemon](https://www.npmjs.com/package/nodemon) | A library to automatically restart node application | 2.0.16  |

## API's used

| API                                             | Description                                               | Used in Page   |
| ----------------------------------------------- | --------------------------------------------------------- | -------------- |
| [Multiavatar API](https://api.multiavatar.com/) | API to get random avatars for profile image               | SetAvatar Page |
| [Edamam's Recipe API](https://www.edamam.com/)  | API to get recipes of the searched ingredients/food-items | Diet Page      |

## 👦 Author

[![LinkedIn](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aham-gupta-18a02a202/)
[![GitHub](https://img.shields.io/badge/github-1DA1F2?style=for-the-badge&logo=github&logoColor=white)](https://github.com/aham-18113)
