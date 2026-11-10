# GSO Asset and Inventory Management System

Central repository for the Web-Based Asset and Inventory Management System with QR Code Tracking and Automated Reporting for the General Services Office (GSO) of El Salvador City Hall.

## Project Repositories

- **Frontend:** [gso_frontend](https://github.com/AaronMicarte/gso_frontend)
- **Backend:** [gso_backend](https://github.com/AaronMicarte/gso_backend)
- **Mobile:** [gso_mobile](https://github.com/AaronMicarte/gso_mobile)

## Prerequisites

Make sure the following tools are installed:

- [Git](https://git-scm.com/)
- [Node.js and npm](https://nodejs.org/)
- [PHP](https://www.php.net/)
- [Composer](https://getcomposer.org/)
- [MySQL](https://www.mysql.com/)
- [Expo Go](https://expo.dev/client) (for mobile testing)

## Setup and Installation

### 1. Clone the Repositories

Clone each repository separately:

```bash
git clone https://github.com/AaronMicarte/gso_frontend.git
git clone https://github.com/AaronMicarte/gso_backend.git
git clone https://github.com/AaronMicarte/gso_mobile.git
```

### 2. Backend Setup (Laravel)

Navigate to the backend directory:

```bash
cd gso_backend
composer install
```

Configure your `.env` file using `.env.example` as a reference.

Generate the application key:

```bash
php artisan key:generate
```

Create the required MySQL database and configure its connection details in `.env`.

Run database migrations:

```bash
php artisan migrate
```

Start the backend server:

```bash
php artisan serve
```

### 3. Frontend Setup (Next.js)

Open a new terminal and navigate to the frontend directory:

```bash
cd gso_frontend
npm install
```

Configure the required environment variables using `.env.example` as a reference, including the backend API URL.

Start the development server:

```bash
npm run dev
```

### 4. Mobile Setup (Expo)

Open another terminal and navigate to the mobile directory:

```bash
cd gso_mobile
npm install
```

Configure the backend API URL in the mobile application's environment configuration.

Start the Expo development server:

```bash
npx expo start
```

Scan the QR code using Expo Go to run the application on a mobile device.

## Running the System

Run the three components independently in separate terminals:

| Component | Command | Default Address |
|---|---|---|
| Backend | `php artisan serve` | http://127.0.0.1:8000 |
| Frontend | `npm run dev` | http://localhost:3000 |
| Mobile | `npx expo start` | Expo development server |

**Note:** Make sure the MySQL database is running and the backend API is accessible before using the frontend or mobile application.


**Project:** GSO Asset and Inventory Management System  
**Organization:** General Services Office (GSO), El Salvador City Hall
