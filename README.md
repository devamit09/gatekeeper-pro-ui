# GateKeeper Pro - Frontend

An Angular frontend for GateKeeper Pro that integrates with a Spring Boot backend using JWT-based authentication.

## Features

- JWT login/register with secure token storage
- Angular Material UI
- Protected dashboard route with AuthGuard
- Fully responsive design

## Tech Stack

- Angular 17+
- Angular Material
- RxJS
- TypeScript
- JWT
- SCSS styling

## Getting Started

### Prerequisites

- Node.js and npm installed
- Angular CLI (`npm install -g @angular/cli`)
- Backend running on `http://localhost:8080`

### Installation

```bash
npm install
```

### Run Development Server

```bash
ng serve
```

Access the app at: [http://localhost:4200](http://localhost:4200)

### Routing

| Route        | Description          |
|--------------|----------------------|
| `/login`     | Login form           |
| `/register`  | Register form        |
| `/dashboard` | Protected dashboard  |

### Build for Production

```bash
ng build
```

### Authentication Flow

- On login, JWT token is received and stored in localStorage.
- AuthGuard ensures protected routes.
- Token is sent in `Authorization` header for secure API requests.

## Screenshots

Dashboard view:

```
+-------------------------------------------------+
| GateKeeper Pro Dashboard       [ Logout ]       |
+-------------------------------------------------+
| Welcome to the protected Dashboard!             |
| You are logged in with JWT authentication.      |
+-------------------------------------------------+
```

## Deployment

You can deploy this app to Vercel, Netlify, Firebase Hosting, or serve it via Nginx after running `ng build`.