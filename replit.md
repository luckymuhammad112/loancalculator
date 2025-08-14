# Replit.md

## Overview

LoanCalc Pro is a professional loan calculation web application that provides advanced financial calculation tools for different types of loans and investments. The application features three main calculator types: amortized loans (with fixed monthly payments), deferred payment loans (single lump sum payment), and bond calculators (investment grade calculations). Built with a modern React frontend and Express.js backend, the application offers real-time calculations, interactive charts, and comprehensive educational content for users to understand loan mechanics.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript using Vite as the build tool
- **UI Components**: Shadcn/ui component library with Radix UI primitives for consistent, accessible interface components
- **Styling**: Tailwind CSS with custom CSS variables for theming, supporting both light and dark modes
- **State Management**: React Query (TanStack Query) for server state management and caching
- **Routing**: Wouter for lightweight client-side routing
- **Charts**: Recharts library for interactive financial data visualization
- **Forms**: React Hook Form with Zod validation for type-safe form handling

### Backend Architecture
- **Framework**: Express.js with TypeScript running on Node.js
- **Database ORM**: Drizzle ORM with PostgreSQL dialect for type-safe database operations
- **Schema Validation**: Zod schemas shared between frontend and backend for consistent data validation
- **Storage Layer**: Abstracted storage interface with in-memory implementation for development, designed to easily switch to database persistence
- **API Design**: RESTful API endpoints following conventional HTTP methods and status codes

### Core Features
- **Calculator Types**: Three distinct calculation engines for amortized loans, deferred payments, and bonds
- **Real-time Calculations**: Instant calculation updates as users modify input parameters
- **Data Persistence**: Calculator results are saved to track usage patterns and provide analytics
- **Educational Content**: CMS-like system for articles and FAQ content to improve SEO and user education
- **Responsive Design**: Mobile-first approach with adaptive layouts for all screen sizes

### SEO and Content Strategy
- **Server-side Rendering**: Helmet integration for dynamic meta tags and structured data
- **Content Management**: Database-driven articles and FAQ system with slug-based routing
- **Schema Markup**: JSON-LD structured data for better search engine understanding
- **Performance Optimization**: Lazy loading, code splitting, and optimized asset delivery

## External Dependencies

### Database
- **Neon Database**: Serverless PostgreSQL database service via `@neondatabase/serverless`
- **Database Migrations**: Drizzle Kit for schema migrations and database management

### UI and Styling
- **Shadcn/ui**: Component library built on Radix UI primitives
- **Radix UI**: Comprehensive set of accessible UI components
- **Tailwind CSS**: Utility-first CSS framework with PostCSS processing
- **Lucide React**: Icon library for consistent iconography

### Development Tools
- **Vite**: Build tool and development server with HMR support
- **TypeScript**: Static type checking across the entire application
- **ESBuild**: Fast JavaScript bundling for production builds
- **Replit Integration**: Development environment optimization with Replit-specific plugins

### Third-party Services
- **Google Fonts**: Web fonts (Inter, DM Sans, Fira Code, Geist Mono, Architects Daughter)
- **Unsplash**: Stock photography for article images and visual content
- **AdSense Integration**: Prepared advertising zones for monetization (placeholder implementation)

### Data Visualization
- **Recharts**: React chart library for pie charts and financial data visualization
- **Embla Carousel**: Touch-friendly carousel component for content galleries

### Form Handling and Validation
- **React Hook Form**: Performant form library with minimal re-renders
- **Hookform Resolvers**: Integration layer for validation schema resolvers
- **Zod**: TypeScript-first schema validation library used across frontend and backend