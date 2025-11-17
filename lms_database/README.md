# TechLearn LMS Database (MongoDB)

This container represents the MongoDB database used by the LMS.

- The backend connects using standard MongoDB URI and database name read from environment variables.
- No database commands are executed here; provisioning is performed externally.

## Environment Variables (used by backend)
- MONGO_URI or MONGODB_URL (depending on environment)
- MONGO_DB_NAME or MONGODB_DB

The FastAPI backend expects:
- MONGO_URI
- MONGO_DB_NAME

Map your environment's values accordingly (e.g., in docker compose env or deployment configuration).
