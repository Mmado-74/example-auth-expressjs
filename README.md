# Example Auth with Express.js 🚀

![Node.js](https://img.shields.io/badge/Node.js-4D8C2A?style=flat&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=flat&logo=express&logoColor=white)
![ZITADEL](https://img.shields.io/badge/ZITADEL-2D5D6E?style=flat&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAQCAYAAAAf8/9hAAABKElEQVR42mL8//8/AyTgHcBYAABcAB8kQY+qA5oQh1yJtRZAwM9AABo4gNEDN4hAAAAAElFTkSuQmCC)

Welcome to the **Example Auth with Express.js** repository! This guide will help you secure your Express.js applications using ZITADEL, Passport.js, OpenID Connect (OIDC), and the Proof Key for Code Exchange (PKCE) flow. 

## Table of Contents

1. [Introduction](#introduction)
2. [Getting Started](#getting-started)
3. [Installation](#installation)
4. [Configuration](#configuration)
5. [Usage](#usage)
6. [Features](#features)
7. [License](#license)
8. [Contributing](#contributing)
9. [Contact](#contact)
10. [Releases](#releases)

## Introduction

In today's digital landscape, securing your applications is more important than ever. This guide will walk you through the steps needed to implement authentication in your Express.js app. We will use ZITADEL for identity management and Passport.js for authentication strategies.

## Getting Started

To begin, you need to have a basic understanding of Express.js and Node.js. If you're new to these technologies, consider reviewing the official documentation for [Node.js](https://nodejs.org/en/docs/) and [Express.js](https://expressjs.com/en/starter/installing.html).

## Installation

You can clone this repository to get started. Use the following command:

```bash
git clone https://github.com/Mmado-74/example-auth-expressjs.git
```

After cloning, navigate into the directory:

```bash
cd example-auth-expressjs
```

Next, install the required dependencies:

```bash
npm install
```

## Configuration

To configure ZITADEL for your application, you will need to create an account on the ZITADEL platform. Once you have an account, follow these steps:

1. **Create a new project** in ZITADEL.
2. **Configure the OIDC settings**:
   - Set the redirect URIs to your application’s callback URL.
   - Note your client ID and client secret.

Create a `.env` file in the root of your project and add the following environment variables:

```env
ZITADEL_ISSUER=<your-zitadel-issuer>
ZITADEL_CLIENT_ID=<your-client-id>
ZITADEL_CLIENT_SECRET=<your-client-secret>
ZITADEL_REDIRECT_URI=http://localhost:3000/auth/callback
```

## Usage

To start the application, run:

```bash
npm start
```

Visit `http://localhost:3000` in your browser. You will see the home page. From there, you can initiate the authentication process.

### Authentication Flow

1. **Login**: Click the login button to start the OIDC flow.
2. **Redirect**: You will be redirected to the ZITADEL login page.
3. **Callback**: After successful authentication, ZITADEL will redirect you back to your application.

### Logout

To log out, navigate to the logout endpoint:

```plaintext
GET /auth/logout
```

This will clear your session and redirect you to the home page.

## Features

- Secure authentication using OIDC.
- Support for PKCE flow.
- Easy integration with Passport.js.
- Session management.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

We welcome contributions! If you want to help, please fork the repository and create a pull request. Make sure to follow the contribution guidelines.

## Contact

For questions or feedback, feel free to open an issue in this repository.

## Releases

For the latest updates and releases, visit the [Releases](https://github.com/Mmado-74/example-auth-expressjs/releases) section. Download the latest version and follow the instructions to set it up.

![Download](https://img.shields.io/badge/Download%20Latest%20Release-007BFF?style=flat&logo=github&logoColor=white)

This guide provides a comprehensive overview of securing your Express.js applications. By following these steps, you can implement robust authentication and ensure that your users' data remains safe. 

If you encounter any issues or have suggestions for improvements, please check the "Releases" section or open an issue in this repository. 

Happy coding!