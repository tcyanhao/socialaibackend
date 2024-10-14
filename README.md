The SocialAI backend handles all image generation requests, storage, and search functionality. The backend was developed in Go and integrates with OpenAI's DALL-E 3 API for image generation, Google Cloud Storage for storing user-uploaded images, and Elasticsearch for efficient image search.

Features
Image Generation: Uses OpenAI's DALL-E 3 API to generate images based on natural language descriptions.
Image Storage: Stores generated images in Google Cloud Storage and manages storage operations.
Search Functionality: Implements fast, keyword-based image search using Elasticsearch to index and retrieve images efficiently.

Project Structure
backend/
  ├── elasticsearch.go   # Handles Elasticsearch integration for searching images.
  ├── gsc.go             # Manages Google Cloud Storage (GCS) interactions for image storage.
constants/
  ├── constants.go       # Contains global constants used across the project.
handler/
  ├── post.go            # Handles API requests related to image generation.
  ├── router.go          # Defines API routes and request handling.
  ├── user.go            # Handles API requests related to user authentication and management.
model/
  ├── model.go           # Defines data models (e.g., Post, User) used in the system.
service/
  ├── post.go            # Business logic for image generation and storage.
  ├── user.go            # Business logic for user authentication and management.
app.yaml                 # Google Cloud App Engine configuration.
go.mod                   # Go module dependencies.
go.sum                   # Dependency checksums.
main.go                  # Main entry point for the backend service.

Local Development
Clone the repository: https://github.com/tcyanhao/socialaibackend.git
