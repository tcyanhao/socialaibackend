The SocialAI backend handles all image generation requests, storage, and search functionality. The backend was developed in Go and integrates with OpenAI's DALL-E 3 API for image generation, Google Cloud Storage for storing user-uploaded images, and Elasticsearch for efficient image search.

Features
Image Generation: Uses OpenAI's DALL-E 3 API to generate images based on natural language descriptions.
Image Storage: Stores generated images in Google Cloud Storage and manages storage operations.
Search Functionality: Implements fast, keyword-based image search using Elasticsearch to index and retrieve images efficiently.

Project Structure
/backend: Contains core backend logic.

elasticsearch.go: Manages the integration with Elasticsearch for image search functionality.
gsc.go: Handles interactions with Google Cloud Storage (GCS) for image uploads and retrieval.
/constants: Stores global constants used throughout the project.

constants.go: Contains configuration constants and reusable values.
/handler: Contains request handlers and API route logic.

post.go: Manages API requests related to posts and image generation.
router.go: Defines API routes and their handlers.
user.go: Handles API requests related to user management, including signup and login.
/model: Defines the data models used by the application.

model.go: Includes data structures for posts, users, and other entities.
/service: Contains the business logic for processing data and managing application workflows.

post.go: Implements the core logic for image generation and storage services.
user.go: Implements the core logic for user management and authentication.
app.yaml: Configuration file for deploying the backend to Google Cloud App Engine.

go.mod: Specifies the Go module dependencies for the project.

go.sum: Contains checksums of dependencies to ensure integrity.

main.go: Entry point for the application, initializing routes and starting the server.

Local Development
Clone the repository: https://github.com/tcyanhao/socialaibackend.git
