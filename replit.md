# Portfolio Application

## Overview

This is a modern, responsive portfolio website built for Samiksha Magdum, a Computer Science Engineering student. The application is a full-stack React/Express application with a sophisticated UI built using shadcn/ui components, modern styling with Tailwind CSS, and a PostgreSQL database backend using Drizzle ORM.

## System Architecture

The application follows a monorepo structure with clear separation between client, server, and shared code:

- **Frontend**: React with TypeScript, built using Vite
- **Backend**: Express.js server with TypeScript
- **Database**: PostgreSQL with Drizzle ORM
- **Styling**: Tailwind CSS with custom design system
- **UI Components**: shadcn/ui component library
- **Routing**: Wouter for client-side routing
- **State Management**: TanStack Query for server state

## Key Components

### Frontend Architecture
- **React SPA**: Single-page application with component-based architecture
- **Component Structure**: Organized into sections (Hero, About, Skills, Projects, Experience, Contact)
- **Design System**: Custom color palette with CSS variables for theming
- **Responsive Design**: Mobile-first approach with Tailwind CSS
- **Modern UI**: Glassmorphism effects, gradients, and smooth animations

### Backend Architecture
- **Express Server**: RESTful API structure with middleware for logging and error handling
- **Database Layer**: Abstracted storage interface with in-memory implementation for development
- **Development Tools**: Hot reload with Vite integration for development environment

### Database Schema
- **Users Table**: Basic user model with id, username, and password fields
- **Extensible Design**: Schema designed to accommodate future portfolio-related entities

## Data Flow

1. **Client Requests**: React components make API calls using TanStack Query
2. **Server Processing**: Express routes handle requests and interact with storage layer
3. **Database Operations**: Drizzle ORM provides type-safe database interactions
4. **Response**: Data flows back through the same path with proper error handling

## External Dependencies

### Core Technologies
- **React Ecosystem**: React 18 with hooks, TanStack Query for data fetching
- **UI Framework**: Radix UI primitives with shadcn/ui wrapper components
- **Styling**: Tailwind CSS with PostCSS processing
- **Database**: Neon PostgreSQL (serverless) with Drizzle ORM
- **Build Tools**: Vite for frontend bundling, ESBuild for server compilation

### Development Tools
- **TypeScript**: Full type safety across client and server
- **Development Server**: Vite with HMR and custom middleware
- **Code Quality**: ESLint configuration through shadcn/ui setup

## Deployment Strategy

### Build Process
- **Frontend**: Vite builds optimized production bundle to `dist/public`
- **Backend**: ESBuild compiles TypeScript server to `dist/index.js`
- **Database**: Drizzle migrations handle schema changes

### Environment Configuration
- **Development**: Local development with Vite dev server proxy
- **Production**: Static files served by Express with API routes
- **Database**: Environment-based DATABASE_URL configuration

### Replit Integration
- **Development Banner**: Automatic Replit development environment detection
- **Runtime Error Handling**: Replit-specific error overlay for development
- **Cartographer Integration**: Code mapping for enhanced debugging

## Changelog

```
Changelog:
- July 01, 2025. Initial setup
```

## User Preferences

```
Preferred communication style: Simple, everyday language.
```