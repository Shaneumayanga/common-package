# COMMONCODE

`COMMONCODE` is a shared development package for building **microservices**. It provides reusable utilities such as custom error classes and middleware functions for Express.js applications.

## Folder Structure

```
COMMONCODE/
├── src/
│   ├── errors/
│   │   ├── bad-request-error.ts          # 400 Bad Request errors
│   │   ├── custom-error.ts               # Base custom error class
│   │   ├── database-connection-error.ts  # Database connectivity errors
│   │   ├── not-authorized-error.ts       # 401 Unauthorized errors
│   │   ├── not-found-error.ts            # 404 Not Found errors
│   │   └── request-validation-error.ts   # Request validation errors
│   ├── middlewares/
│   │   ├── current-user.ts              # User authentication middleware
│   │   ├── error-handler.ts             # Global error handling middleware
│   │   ├── require-auth.ts              # Authorization middleware
│   │   └── validate-request.ts          # Request validation middleware
│   └── index.ts                         # Main entry point / exports
```

## Features

### Errors

Custom error classes for common scenarios:

- **BadRequestError** – 400 Bad Request
- **DatabaseConnectionError** – Database connection failures
- **NotAuthorizedError** – 401 Unauthorized
- **NotFoundError** – 404 Not Found
- **RequestValidationError** – Invalid request payloads
- **CustomError** – Base class for all custom errors

### Middlewares

Reusable Express middleware functions:

- **currentUser** – Extracts authenticated user info from requests
- **errorHandler** – Global error handler for consistent error responses
- **requireAuth** – Protects routes that require authentication
- **validateRequest** – Validates incoming requests against defined rules



