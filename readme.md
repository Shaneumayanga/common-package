Common development package that i use when microservices development

COMMONCODE/
├── src/                           # Source code
│   ├── errors/                    # Custom error definitions
│   │   ├── bad-request-error.ts          # 400 Bad Request errors
│   │   ├── custom-error.ts               # Base custom error class
│   │   ├── database-connection-error.ts  # Database connectivity error
│   │   ├── not-authorized-error.ts       # 401 Unauthorized errors
│   │   ├── not-found-error.ts            # 404 Not Found errors
│   │   └── request-validation-error.ts   # Request validation errors
│   ├── middlewares/               # Express middleware functions
│   │   ├── current-user.ts              # User authentication middleware
│   │   ├── error-handler.ts             # Global error handling middleware
│   │   ├── require-auth.ts              # Authorization middleware
│   │   └── validate-request.ts          # Request validation middleware
│   └── index.ts                   # Main entry point/exports
