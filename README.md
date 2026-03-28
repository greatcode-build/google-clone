# Google Clone

A modern, responsive Google search clone built with Next.js, featuring web and image search capabilities, dark/light theme support, and seamless user experience.

## 🚀 What This Project Does

This application replicates the core functionality of Google's search engine, allowing users to perform web searches and image searches. It provides a clean, intuitive interface with features like pagination, theme switching, and random search suggestions.

## ✨ Key Features

- **Web Search**: Perform comprehensive web searches with results displayed in a familiar Google-like format
- **Image Search**: Search and browse images with thumbnail previews
- **Dark/Light Theme**: Toggle between dark and light modes for comfortable viewing
- **Pagination**: Navigate through search results with numbered pagination buttons
- **Random Search**: Discover new content with a random word search feature
- **Responsive Design**: Optimized for desktop and mobile devices
- **Google OAuth Integration**: Secure authentication using Google accounts

## 🛠️ Tech Stack

- **Framework**: Next.js 16 with App Router
- **Language**: TypeScript
- **Styling**: Tailwind CSS 4
- **Authentication**: NextAuth.js with Google Provider
- **Icons**: React Icons
- **API**: Google Custom Search API

## 📋 Prerequisites

Before you begin, ensure you have:

- Node.js (version 18 or higher)
- npm or yarn package manager
- Google Cloud Console account for API access

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/google-clone.git
cd google-clone
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Set Up Environment Variables

Create a `.env.local` file in the root directory and add your Google API credentials:

```env
GOOGLE_API_KEY=your_google_api_key_here
CONTEXT_KEY=your_custom_search_engine_id_here
NEXTAUTH_SECRET=your_nextauth_secret_here
NEXTAUTH_URL=http://localhost:3000
```

#### Getting Google API Credentials:

1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create a new project or select an existing one
3. Enable the Custom Search JSON API
4. Create credentials (API Key)
5. Set up a Custom Search Engine at [Google Custom Search](https://cse.google.com/)
6. Get your Search Engine ID (cx parameter)

### 4. Run the Development Server

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to see the application.

### 5. Build for Production

```bash
npm run build
npm start
```

## 📖 Usage Examples

### Performing a Search

1. Enter your search query in the search box on the homepage
2. Press Enter or click the search icon
3. Switch between "All" (web results) and "Images" tabs

### Random Search

- Click the "I'm Feeling Lucky" style button for a random search

### Theme Toggle

- Use the theme switcher in the header to toggle between light and dark modes

## 🏗️ Project Structure

```
google-clone/
├── app/
│   ├── api/auth/[...nextauth]/    # Authentication routes
│   ├── components/                # Reusable UI components
│   ├── search/
│   │   ├── web/                   # Web search page
│   │   └── image/                 # Image search page
│   ├── layout.tsx                 # Root layout
│   └── page.tsx                   # Homepage
├── auth.ts                        # Authentication configuration
├── tailwind.config.ts             # Tailwind CSS configuration
└── package.json                   # Project dependencies
```
