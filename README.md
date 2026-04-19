# Secrets API CRUD Client

A Node.js web application that demonstrates how to interact with a RESTful API using **Axios**. This project performs full CRUD (Create, Read, Update, Delete) operations to manage "secrets" data via a remote server.

## 🚀 Features

- **GET**: Retrieve a specific secret by its ID.
- **POST**: Create a new secret.
- **PUT**: Fully update an existing secret.
- **PATCH**: Partially update an existing secret.
- **DELETE**: Remove a secret from the database.
- **Authentication**: Implements Bearer Token authentication for secure API requests.

## 🛠️ Technologies Used

- **Node.js**: JavaScript runtime environment.
- **Express.js**: Web framework for the server-side logic.
- **Axios**: Promise-based HTTP client for the browser and node.js.
- **EJS**: Embedded JavaScript templates for rendering the frontend.
- **Body-Parser**: Middleware to handle incoming request bodies.

## 📋 Prerequisites

Before you begin, ensure you have the following installed:
- [Node.js](https://nodejs.org/) (v14.0 or higher)
- npm (Node Package Manager)

## 🔧 Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/zunayeed/secrets-api-crud-client.git](https://github.com/zunayeed/secrets-api-crud-client.git)
   cd secrets-api-crud-client

   Install dependencies:

Bash
npm install
Configure Authentication:
Open index.js and locate the yourBearerToken variable. Replace the placeholder with your valid API token:

JavaScript
const yourBearerToken = "YOUR_ACTUAL_TOKEN_HERE";
Start the server:

Bash
node index.js
View the app:
Open your browser and navigate to http://localhost:3000.

📖 How It Works
This client communicates with the App Brewery Secrets API.

Key Endpoints Managed:
GET /secrets/:id - Fetches data using the config object containing the Authorization header.

POST /secrets - Sends a JSON body to create a new entry.

PUT/PATCH /secrets/:id - Updates entries based on the ID provided in the form.

DELETE /secrets/:id - Removes entries using the DELETE HTTP method.

⚠️ Important Note
This project is for educational purposes. Do not commit your real Bearer Token to a public repository. Consider using a .env file and dotenv package for production-level security.

📄 License
This project is open source and available under the MIT License.
