# Atria SaaS Application - README

## Overview
Atria is a SaaS application designed to help users ship winning ads 10 times faster. It provides a proven system for consistently creating winning ads, moving beyond guesswork. Top customers are already experiencing a 40% uplift in performance and a 25% reduction in customer acquisition cost (CAC).

## Core Features

### 1. AI-Powered Algorithm: Radar
- Trained on over a billion in ad spend
- Acts as an always-on ad optimizer
- Scores and refines creatives with real-world data
- Helps spot iteration opportunities immediately
- Provides actionable insights

### 2. Competitor Spying Tool
- Reverse engineer strategies of top brands
- Uncover top hooks, themes, emotions, desires, ad angles, and personas
- Transcribe video scripts of competitor ads
- Generate readymade scripts based on landing pages

### 3. Creative Reporting Tool
- Comprehensive reporting for ad creatives
- Configure attribution settings
- Share reports for team collaboration
- Compare performance against averages
- Customize columns and views
- AI-powered tagging of top creatives

### 4. Customer Review Mining Tool
- AI analysis of customer reviews/feedback
- Upload spreadsheets from sources like Trustpilot
- Analyze audiences and their preferences
- Suggest ad concepts based on customer feedback
- Keyword analysis for testimonials

## Technical Implementation

### Frontend
- Next.js with TypeScript
- React components with Tailwind CSS
- Responsive design for all devices

### Backend
- Next.js API routes
- Notion integration for data storage
- OpenAI integration for AI features

## Getting Started

### Local Development
1. Clone the repository
2. Install dependencies: `npm install`
3. Copy `.env.example` to `.env.local` and fill in your API keys:
   ```
   NOTION_API_KEY=your_notion_api_key_here
   NOTION_ADS_DATABASE_ID=your_notion_ads_database_id_here
   NOTION_COMPETITORS_DATABASE_ID=your_notion_competitors_database_id_here
   NOTION_REVIEWS_DATABASE_ID=your_notion_reviews_database_id_here
   OPENAI_API_KEY=your_openai_api_key_here
   ```
4. Run the development server: `npm run dev`
5. Open [http://localhost:3000](http://localhost:3000) in your browser

### Notion Setup
1. Create a Notion integration at https://www.notion.so/my-integrations
2. Create the following databases in your Notion workspace:
   - Ads Database
   - Competitors Database
   - Reviews Database
3. Share each database with your integration
4. Copy the database IDs and add them to your environment variables

### Deployment

#### Vercel Deployment
1. Fork this repository to your GitHub account
2. Create a new project on Vercel and connect it to your GitHub repository
3. Add the required environment variables in the Vercel project settings
4. Deploy the project

#### Replit Deployment
1. Create a new Replit project
2. Import the GitHub repository
3. Set the environment variables in the Replit secrets
4. Run `npm install` and then `npm run build`
5. Start the server with `npm start`

## Project Structure

- `/src/app` - Next.js app router pages
- `/src/app/api` - API routes for backend functionality
- `/src/components` - Reusable UI components
- `/src/lib` - Utility functions and API clients
- `/src/types` - TypeScript type definitions
- `/src/hooks` - Custom React hooks
- `/src/styles` - Global styles

## API Routes

- `/api/ads` - CRUD operations for ads
- `/api/competitors` - Competitor analysis
- `/api/reviews` - Customer review mining
- `/api/reports` - Reporting and analytics
- `/api/generate` - AI-powered content generation

## License
This project is proprietary and confidential.
