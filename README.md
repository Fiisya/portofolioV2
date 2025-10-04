# Portfolio Project 🚀

This project is a dynamic portfolio website that fetches user and repository data directly from the GitHub API. It leverages Node.js, Express, and Axios to create a server-side application that serves a dynamically generated `index.html` file. The application is designed to be deployed on Vercel as a serverless function, providing a scalable and cost-effective solution for hosting a personal portfolio. It solves the problem of manually updating a portfolio by automatically pulling the latest information from GitHub.

## 🚀 Key Features

- **Dynamic Content**: Fetches user and repository data directly from the GitHub API, ensuring the portfolio is always up-to-date. 🔄
- **Serverless Deployment**: Designed for deployment on Vercel as a serverless function, offering scalability and cost-efficiency. ☁️
- **Express Server**: Uses Express.js to handle routing and serve the portfolio website. 🌐
- **API Endpoint**: Provides an API endpoint (`/api/github-data`) for retrieving raw GitHub data in JSON format. ⚙️
- **Environment Variable Support**: Utilizes `.env` files to manage sensitive information like API keys. 🔑
- **Automatic Updates**: Automatically restarts the server during development when file changes are detected using Nodemon. 🔄
- **Error Handling**: Implements robust error handling to provide informative responses to the user. ⚠️

## 🛠️ Tech Stack

- **Backend**:
    - Node.js
    - Express.js
- **HTTP Client**:
    - Axios
- **Environment Variables**:
    - dotenv
- **Deployment**:
    - Vercel
    - `@vercel/node` builder
- **Development Tools**:
    - Nodemon
- **Other**:
    - path (Node.js module)
    - url (Node.js module)

## 📦 Getting Started / Setup Instructions

### Prerequisites

- Node.js (>=14)
- npm or yarn
- A GitHub account (for accessing the GitHub API)

### Installation

1.  Clone the repository:

    ```bash
    git clone <repository-url>
    cd portfolio
    ```

2.  Install dependencies:

    ```bash
    npm install  # or yarn install
    ```

3.  Create a `.env` file in the root directory and add your GitHub username:

    ```
    GITHUB_USERNAME=your_github_username
    ```

    *Note: You might need a GitHub API token if you exceed the unauthenticated rate limit. If so, add it to your `.env` file as `GITHUB_TOKEN=your_github_token`*

### Running Locally

1.  Start the development server:

    ```bash
    npm run dev  # or yarn dev
    ```

    This will start the server using Nodemon, which automatically restarts the server when file changes are detected.

2.  Open your browser and navigate to `http://localhost:3000` to view the portfolio.

## 💻 Usage

Once the server is running, the portfolio website will be accessible at `http://localhost:3000`. The website dynamically fetches data from the GitHub API and displays it. You can also access the raw GitHub data via the `/api/github-data` endpoint.

## 📂 Project Structure

```
portfolio/
├── public/
│   ├── index.html
│   └── ... (other static files)
├── server.js
├── package.json
├── vercel.json
└── .env
```

## 📸 Screenshots

(Add screenshots of your portfolio website here)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues to suggest improvements or report bugs.

## 📝 License

This project is licensed under the [MIT License](LICENSE) - see the `LICENSE` file for details.

## 📬 Contact

If you have any questions or suggestions, feel free to contact me at [your-email@example.com](mailto:your-email@example.com).

## 💖 Thanks Message

Thank you for checking out this project! I hope it's helpful and inspires you to create your own dynamic portfolio.
