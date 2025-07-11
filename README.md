# LÖTUS Pilates Retreat - Complete Documentation

Welcome to the comprehensive documentation for the LÖTUS Pilates retreat platform. This documentation covers all aspects of the website that sells exclusive wellness and pilates retreats, from technical implementation to user experience design.

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Documentation Structure](#documentation-structure)
- [Quick Navigation](#quick-navigation)
- [Getting Started](#getting-started)
- [Key Features](#key-features)
- [Technical Architecture](#technical-architecture)
- [Contributing](#contributing)

## 🌟 Project Overview

LÖTUS is an exclusive wellness and pilates retreat website that offers transformative experiences in stunning natural locations. The platform combines:

- **Immersive Landing Page**: Video hero sections with helicopter arrivals and wellness footage
- **The LÖTUS Experience**: Curated content emphasizing commitment, exclusivity, health, care, natural beauty, and harmony
- **Next Event Showcase**: Dynamic retreat presentations with villa carousels and booking integration
- **Comprehensive Booking System**: Full-featured reservation and payment processing

## 📚 Documentation Structure

### Core Documentation

- **[Introduction](introduction.mdx)** - Platform overview and key features
- **[Architecture](architecture.mdx)** - Technical system design and patterns
- **[Getting Started](getting-started.mdx)** - Quick setup guide for developers

### Landing Page Components

#### Primary Components
- **[Hero Section](components/hero-section.mdx)** - Video/image hero with LÖTUS branding
- **[LÖTUS Experience](components/lotus-experience.mdx)** - Brand values and service showcase
- **[Next Event](components/next-event.mdx)** - Retreat presentation with villa carousels
- **[Booking Widget](components/booking-widget.mdx)** - Complete reservation system

#### UI Components
- **[Carousel](components/carousel.mdx)** - Versatile image and content slider
- **[CTA Button](components/cta-button.mdx)** - Branded call-to-action buttons
- **[Service Cards](components/service-cards.mdx)** - Service presentation cards
- **[Video Player](components/video-player.mdx)** - Optimized video playback

### API Documentation

#### Core APIs
- **[API Introduction](api-reference/introduction.mdx)** - Authentication, rate limiting, and standards
- **[Authentication](api-reference/authentication.mdx)** - JWT-based auth system

#### Booking System
- **[Create Booking](api-reference/bookings/create-booking.mdx)** - Complete booking creation
- **[Get Booking](api-reference/bookings/get-booking.mdx)** - Retrieve booking details
- **[Update Booking](api-reference/bookings/update-booking.mdx)** - Modify existing bookings
- **[Cancel Booking](api-reference/bookings/cancel-booking.mdx)** - Cancellation handling

#### Retreat Management
- **[List Retreats](api-reference/retreats/list-retreats.mdx)** - Comprehensive retreat listings
- **[Get Retreat](api-reference/retreats/get-retreat.mdx)** - Detailed retreat information
- **[Create Retreat](api-reference/retreats/create-retreat.mdx)** - Admin retreat creation

#### User Management
- **[User Registration](api-reference/users/register.mdx)** - Account creation
- **[User Login](api-reference/users/login.mdx)** - Authentication flow
- **[User Profile](api-reference/users/profile.mdx)** - Profile management

### Development Guides

- **[Development Setup](development/setup.mdx)** - Complete environment configuration
- **[Deployment](development/deployment.mdx)** - Production deployment guide
- **[Testing](development/testing.mdx)** - Testing strategies and examples

## 🚀 Quick Navigation

### For Designers & Content Managers
- [Landing Page Vision](#landing-page-vision) - Original French specifications
- [Component Gallery](components/) - All UI components with examples
- [Brand Guidelines](components/lotus-experience.mdx#core-values-integration) - Core vocabulary and values

### For Frontend Developers
- [Component Documentation](components/) - Complete component library
- [Getting Started](getting-started.mdx) - Development setup
- [Hero Section Implementation](components/hero-section.mdx) - Video/image hero setup

### For Backend Developers
- [API Reference](api-reference/) - Complete API documentation
- [Architecture Guide](architecture.mdx) - System design patterns
- [Database Schema](architecture.mdx#database-design) - Data models

### For DevOps & Deployment
- [Development Setup](development/setup.mdx) - Local environment
- [Architecture Overview](architecture.mdx) - Infrastructure design
- [Performance Guidelines](api-reference/retreats/list-retreats.mdx#performance-considerations)

## 🎯 Landing Page Vision

Based on the original French specifications, the landing page includes:

### 1. Hero Section (Page d'accueil)
- **Video Option**: 7-second promotional video featuring:
  - Helicopter arrival footage
  - Underwater barracuda shots
  - Women practicing yoga/pilates in natural settings
  - Freeze frame on "YOUR EXCLUSIVE WELLNESS AND PILATES RETREAT" with LÖTUS logo
- **Static Fallback**: High-quality image with animated logo and tagline

### 2. THE LÖTUS EXPERIENCE
- **Core Vocabulary**: Commitment, Exclusive, Health, Care, Natural beauty, Harmony
- **Service Cards**: Visual presentation of exclusive offerings with icons
- **CTA**: "DISCOVER" button leading to detailed information

### 3. OUR NEXT EVENT
- **Event Details**: Location, dates, and retreat information
- **Villa Carousels**: 
  - Photos of sold-out Villa 17 (Itacaré, Brazil)
  - Photos of available Villa 19 with booking capability
- **CTA**: "BOOK YOUR RETREAT" directing to reservation page

## 🛠 Key Features

### Technical Features
- **Responsive Design**: Mobile-first approach with breakpoint optimization
- **Performance Optimized**: Lazy loading, image optimization, CDN integration
- **Accessibility**: WCAG 2.1 AA compliance with screen reader support
- **SEO Optimized**: Structured data, meta tags, and search engine optimization

### Business Features
- **Real-time Availability**: Live booking availability with WebSocket updates
- **Payment Integration**: Stripe and PayPal with secure processing
- **Multilingual Support**: Content management for multiple languages
- **Analytics**: Comprehensive tracking for business intelligence

### User Experience Features
- **Smooth Animations**: Framer Motion for enhanced interactions
- **Touch Gestures**: Mobile-optimized swipe and touch controls
- **Video Optimization**: Adaptive streaming with fallback options
- **Progressive Enhancement**: Works without JavaScript

## 🏗 Technical Architecture

### Frontend Stack
- **Framework**: Next.js 14 with App Router
- **Styling**: Tailwind CSS with custom design system
- **State Management**: Zustand + React Query
- **Components**: Custom library built on Radix UI
- **Animations**: Framer Motion

### Backend Stack
- **Runtime**: Node.js with Express
- **Database**: PostgreSQL with Prisma ORM
- **Cache**: Redis for session and data caching
- **Authentication**: JWT with refresh tokens
- **Payments**: Stripe integration with webhooks

### Infrastructure
- **Hosting**: Vercel (frontend) + AWS (backend)
- **CDN**: CloudFront for global asset delivery
- **Monitoring**: Sentry for error tracking
- **Analytics**: Google Analytics 4

## 📖 Getting Started

### For Immediate Setup
1. **Clone Repository**: `git clone https://github.com/lotus-retreats/platform.git`
2. **Install Dependencies**: `npm install`
3. **Configure Environment**: Copy `.env.example` to `.env.local`
4. **Start Development**: `npm run dev`

### For Component Development
1. **Explore Components**: Start with [Hero Section](components/hero-section.mdx)
2. **Review Props**: Each component has comprehensive TypeScript interfaces
3. **Check Examples**: All components include usage examples
4. **Test Integration**: Components include testing guidelines

### For API Integration
1. **Authentication**: Review [API Introduction](api-reference/introduction.mdx)
2. **Booking Flow**: Implement [Create Booking](api-reference/bookings/create-booking.mdx)
3. **Error Handling**: Follow standardized error response patterns
4. **Rate Limiting**: Respect API limits and implement proper retries

## 🎨 Design System

### Brand Colors
- **Primary**: `#4A5D23` (Olive Green)
- **Secondary**: `#7B8A3A` (Light Green)
- **Accent**: `#2E3A14` (Dark Green)

### Typography
- **Headings**: Custom LÖTUS brand font
- **Body**: Inter for optimal readability
- **Monospace**: JetBrains Mono for code

### Core Values Vocabulary
The platform emphasizes six key values:
1. **Commitment** - Dedication to transformation
2. **Exclusive** - Premium, personalized experiences  
3. **Health** - Holistic wellness focus
4. **Care** - Individual attention and support
5. **Natural Beauty** - Stunning location settings
6. **Harmony** - Mind-body-spirit balance

## 🤝 Contributing

### Documentation Updates
- **Markdown Format**: All docs use MDX with Mintlify components
- **Obsidian Compatible**: Fully readable in Obsidian with linking
- **Version Control**: Track changes via Git commits
- **Review Process**: All changes require documentation review

### Code Contributions
- **Style Guide**: Follow ESLint and Prettier configurations
- **Testing**: Include unit and integration tests
- **Documentation**: Update relevant docs with code changes
- **Type Safety**: Maintain TypeScript coverage

### Content Management
- **Brand Consistency**: Maintain core vocabulary usage
- **Image Assets**: Optimize all images for web delivery
- **Accessibility**: Include alt text and semantic markup
- **SEO**: Structure content for search optimization

## 📞 Support

### Technical Support
- **Email**: [dev-support@lotus-retreats.com](mailto:dev-support@lotus-retreats.com)
- **Documentation Issues**: Create GitHub issues for doc improvements
- **API Questions**: Reference comprehensive API documentation

### Business Inquiries
- **Partnerships**: [partnerships@lotus-retreats.com](mailto:partnerships@lotus-retreats.com)
- **General Support**: [support@lotus-retreats.com](mailto:support@lotus-retreats.com)

---

## 📄 License

This documentation and codebase are proprietary to LÖTUS Pilates Retreats. All rights reserved.

## 🔄 Version

**Documentation Version**: 1.0.0  
**Last Updated**: January 2024  
**Platform Version**: v1.0.0

---

<div align="center">
  <p><em>Transform your wellness journey with LÖTUS</em></p>
  <p><strong>YOUR EXCLUSIVE WELLNESS AND PILATES RETREAT</strong></p>
</div>
