# Style Board Web Application

A social media web application built with **Next.js** that helps users browse clothing items, discover outfit inspirations, explore trending styles, and purchase the exact products they see. The platform brings together fashion lovers who want to share looks, find deals, and engage with a clothing-focused community.

## Features

### Browse and Discover
- Explore clothing items and outfit inspirations shared by users.
- Search by categories to find styles, pieces, or trends.

### Social Interaction
- Create and upload posts with outfit photos or clothing items.
- Save favorite posts for easy access later.
- Upvote and downvote posts to surface trending content.
- Delete your own posts.

### Shopping Integration
- Find exact products shown in posts.
- View deals and recommendations shared by the community.

### Technical Functionality
- **Next.js App Router** for full-stack capabilities.
- **MongoDB** for storing posts, users, and interactions.
- **Tailwind CSS** for styling.
- **AWS S3 image upload support** (in progress) for scalable media management.

## Tech Stack

- **Framework:** Next.js (TypeScript)
- **Database:** MongoDB
- **Styling:** Tailwind CSS
- **Media Uploads:** AWS S3 (partially integrated)
- **Language:** TypeScript

## Getting Started

### Prerequisites
- Node.js 18 or later
- MongoDB (local or Atlas)
- AWS credentials if using image uploads

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/AdvancedUno/Style_Board_Dev.git
   cd Style_Board_Dev
   npm install
   ```
  2. Set environment variables in a .env.local file:
     ```bash
      MONGODB_URI=<your_mongodb_connection_string>
      AWS_ACCESS_KEY_ID=<your_key>
      AWS_SECRET_ACCESS_KEY=<your_secret>
      AWS_BUCKET_NAME=<your_bucket>
      NEXT_PUBLIC_AWS_REGION=<region>
      ```
3. Run the development server:
```bash
npm run dev
http://localhost:3000
```

```bash
Style_Board_Dev/
│
├── app/
│   ├── feed.tsx                 # Feed page
│   ├── layout.tsx               # Root layout
│   ├── page.tsx                 # Home page
│   └── navbar.tsx               # Navbar component
│
├── api/
│   └── posts/                   # Post API routes
│
├── components/                  # UI components
├── lib/                         # MongoDB + AWS utilities
├── models/                      # Mongoose schemas
├── public/                      # Static assets
├── styles/                      # Global styles
│
├── next.config.mjs
├── tailwind.config.ts
├── package.json
└── README.md
```

## Development Notes
- Feed page added and delete functionality works.
- MongoDB integration and AWS upload logic added in `lib/`.
- Post creation and rendering implemented.
- Navbar and Add Post components included.
- More features are actively in progress.

## Deployment
You can deploy this application using platforms such as **Vercel**, **Netlify**, or any Node-compatible cloud service.

For Next.js, the recommended deployment platform is **Vercel**.

Documentation:  
https://nextjs.org/docs/app/building-your-application/deploying

## License

Licensed under the MIT License.

