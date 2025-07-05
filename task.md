# Pet Finder QR Code Shopify App - Task Tracker

## Phase 1: Infrastructure & Foundation Setup (Week 1)
- [x] Task 1.1: Provision the Contabo VPS (SKIPPED - Using local development)
- [x] Task 1.2: Install Docker and Portainer (MCP) on the VPS (SKIPPED - Using Docker Desktop locally)
- [x] Task 1.3: Create the main docker-compose.yml file defining all services (Nginx, API, database, etc.)
- [x] Task 1.4: Set up the self-hosted Supabase (MCP) instance within Docker
- [x] Task 1.5: Configure Nginx as a reverse proxy to route traffic to the future application services
- [x] Task 1.6: Create the database schema by writing and executing SQL migration files for all the tables described in section 5.3
- [x] Task 1.7: Set up a new GitHub (MCP) repository and a basic CI/CD pipeline using GitHub Actions (MCP) that can build a test Docker image

## Phase 2: Core Backend API Development (Week 2)
- [x] Task 2.1: Set up the Python/FastAPI API project structure
- [x] Task 2.2: Establish a connection from the API to the Supabase PostgreSQL database
- [x] Task 2.3: Implement the pet profile management endpoints (Create, Read, Update, Delete), ensuring they only store non-empty fields
- [x] Task 2.4: Implement image uploading functionality, connecting to Supabase Storage for pet photos
- [x] Task 2.5: Develop the QR code generation service that creates a QR code image and saves it to storage
- [x] Task 2.6: Create the webhook processing endpoint for the Shopify orders/paid event

## Phase 3: Shopify App Frontend Development (Week 3-4)
- [ ] Task 3.1: Set up a Shopify Partner Account (MCP) and create a new app
- [ ] Task 3.2: Develop the app as a Theme App Extension within Shopify
- [ ] Task 3.3: Build the main React component for the "Pet Profile Builder"
- [ ] Task 3.4: Implement the "Template Selection" view (Stage 1)
- [ ] Task 3.5: Build the "Interactive Form Mode" (Stage 2) for one template, with styled inputs embedded within a phone mockup
- [ ] Task 3.6: Build the "Final Preview Mode" (Stage 3), which renders the form data as static text and hides empty fields
- [ ] Task 3.7: Implement the state management to switch between Form Mode and Preview Mode
- [ ] Task 3.8: Implement the "Add to Cart" logic, packaging form data into Shopify line item properties
- [ ] Task 3.9: Replicate tasks 3.5 and 3.6 for the other two templates
- [ ] Task 3.10: Write the script to manage the product page buttons

## Phase 4: Customer & Public Pages Development (Week 5)
- [x] Task 4.1: Set up the Next.js project for the public profile pages
- [x] Task 4.2: Create a dynamic route that fetches pet data from the API based on a URL slug
- [x] Task 4.3: Build the public profile page component that dynamically renders content based on the fetched data
- [x] Task 4.4: Set up the React project for the Customer Portal
- [ ] Task 4.5: Implement the login page and authentication flow connecting to the backend API
- [ ] Task 4.6: Build the customer dashboard page for viewing and managing pets
- [ ] Task 4.7: Re-use the Profile Builder component to create the "Edit Profile" page in the portal

## Phase 5: Integration, Testing & Finalization (Week 6)
- [ ] Task 5.1: Fully implement the orders/paid webhook logic
- [ ] Task 5.2: Set up a Printful account and test the entire flow from checkout to mock order
- [ ] Task 5.3: Implement the customer account creation flow
- [ ] Task 5.4: Implement the scan analytics logging and display the data in the customer portal
- [ ] Task 5.5: Conduct end-to-end testing of the complete system

## Phase 6: Deployment & Launch (Week 7)
- [ ] Task 6.1: Finalize the GitHub Actions (MCP) CI/CD pipeline for automated deployment
- [ ] Task 6.2: Configure domain names and set up production SSL certificates with Nginx
- [ ] Task 6.3: Set up monitoring and health checks for all services
- [ ] Task 6.4: Prepare and submit the app for review on the Shopify App Store (MCP)
- [ ] Task 6.5: Develop documentation for store owners on how to install and configure the app

## Notes
- To mark a task as complete, change `- [ ]` to `- [x]`
- Add additional subtasks as needed during development
- Update this document regularly to track progress