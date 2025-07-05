# Pet Finder QR Code Shopify App

A Shopify app that enables store owners to sell personalized pet ID tags with QR codes.

## Overview

This application allows customers to:
- Create custom pet profiles directly on a Shopify product page
- Receive QR code pet tags manufactured by Printful
- Access a customer portal to manage their pet profiles
- Help lost pets get reunited with their owners through scannable QR codes

## System Architecture

The application consists of several components:
- **FastAPI Backend**: Core business logic and API endpoints
- **Next.js Public Profiles**: Public pet profile pages when QR codes are scanned
- **React Customer Portal**: Web app for customers to manage their pet profiles
- **Supabase**: Database, auth, and storage
- **Redis**: Caching
- **Nginx**: Reverse proxy

## Getting Started

### Prerequisites

- Docker and Docker Compose
- Node.js (for local development)
- Python 3.10+ (for local development)

### Setup

1. Clone the repository

2. Start the application with Docker Compose:

```bash
docker-compose up -d
```

3. Access the following services:

   - API Documentation: http://localhost/
   - Customer Portal: http://localhost/portal/
   - Supabase Studio: http://localhost/studio/
   - API Directly: http://localhost/api/

## Development

### API Backend (FastAPI)

The API backend is located in the `api` directory. It handles:
- Pet profile management
- QR code generation
- Shopify webhooks
- Authentication

### Public Profiles (Next.js)

The public profiles application is located in the `public-profiles` directory. It provides:
- Public pet profile pages
- "Found Pet" reporting

### Customer Portal (React)

The customer portal application is located in the `customer-portal` directory. It offers:
- Pet profile management
- Scan analytics
- Account settings