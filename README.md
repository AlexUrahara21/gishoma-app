# GishomaWellPay

## Overview

**GishomaWellPay** is a comprehensive payroll and workforce management system designed specifically for workers at the Gishoma Peat Power Plant. The application enables employees to easily access their payment information, track attendance, manage leave requests, and stay updated on their compensation in a timely and transparent manner.

## Features

- **Employee Payment Management** - Easy access to payment history, salary details, and payment status
- **Attendance Tracking** - Real-time attendance recording and monitoring
- **Leave Management** - Request and track leave applications
- **Admin Dashboard** - Comprehensive administrative controls for managing employees and payments
- **User Management** - Secure user authentication and profile management
- **Search Functionality** - Quick search capabilities for finding payment and employee information

## Prerequisites

Before you begin, ensure you have the following installed:
- **Node.js** (v12.0 or higher)
- **npm** or **yarn** package manager
- **Git**

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Komezusenge-Bolice/gishoma-app.git
   cd gishoma-app
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure environment variables**
   Create a `.env` file in the root directory and add necessary configuration:
   ```
   NODE_ENV=development
   PORT=3000
   ```

4. **Start the application**
   ```bash
   npm start
   ```

The application will be available at `http://localhost:3000`

## Project Structure

```
gishoma-app/
├── bin/
│   └── www                  # Application entry point
├── routes/
│   ├── index.js            # Home route
│   ├── users.js            # User management routes
│   ├── admin.js            # Admin dashboard routes
│   ├── payment.js          # Payment routes
│   ├── attendance.js       # Attendance tracking routes
│   └── leaves.js           # Leave management routes
├── views/
│   ├── layout.jade         # Main layout template
│   ├── index.jade          # Home page
│   └── error.jade          # Error page
├── public/
│   ├── stylesheets/
│   │   └── style.css       # Application styles
│   ├── javascripts/        # Client-side scripts
│   └── images/             # Project images
├── app.js                  # Express application configuration
├── package.json            # Project dependencies
└── README.md              # This file
```

## Technologies Used

- **Backend Framework:** Express.js
- **Template Engine:** Jade (Pug)
- **Node.js Runtime:** v12+
- **Package Manager:** npm/yarn
- **Middleware:**
  - express-json: JSON body parser
  - cookie-parser: Cookie handling
  - morgan: HTTP request logger
  - http-errors: Error handling

## Usage

### Starting the Server
```bash
npm start
```

### Available Routes
- `/` - Home page
- `/users` - User management
- `/admin` - Admin dashboard
- `/payment` - Payment management
- `/attendance` - Attendance tracking
- `/leaves` - Leave management

## Development

For development with auto-reload functionality, consider installing and using `nodemon`:

```bash
npm install --save-dev nodemon
```

Then update the start script in `package.json`:
```json
"scripts": {
  "start": "node ./bin/www",
  "dev": "nodemon ./bin/www"
}
```

Run in development mode:
```bash
npm run dev
```

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Future Enhancements

- Mobile app integration
- Real-time payment notifications
- Advanced analytics and reporting
- Biometric attendance integration
- Multi-language support

## Troubleshooting

### Port Already in Use
If port 3000 is already in use, change it in the `.env` file:
```
PORT=3001
```

### Dependencies Not Installing
Try clearing npm cache:
```bash
npm cache clean --force
npm install
```

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact & Support

For issues, questions, or feedback regarding GishomaWellPay:
- **GitHub Issues:** [Report bugs and request features](https://github.com/Komezusenge-Bolice/gishoma-app/issues)
- **Email:** [Project Maintainer Contact]

## Author

**Komezusenge Bolice**

---

**Last Updated:** January 28, 2026

Thank you for using GishomaWellPay! We're committed to making payroll management simple and efficient for Gishoma Peat Power Plant workers.
