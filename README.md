# YouTube Video Creator

A Next.js application for creating short YouTube videos with AI assistance, specifically optimized for ethical hacking tutorials.

## Features

- **AI-Powered Script Generation**: Create compelling video scripts based on your topic
- **Video Creation**: Transform scripts into professional videos using AI
- **Ethical Hacking Focus**: Specialized tools for cybersecurity content creation
- **Modern UI**: Clean, responsive interface built with Tailwind CSS and shadcn/ui

## Getting Started

### Prerequisites

- Node.js 18+
- npm, yarn, or pnpm

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd youtube-video-creator
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   ```bash
   cp .env.example .env.local
   ```
   Then edit `.env.local` and add your API keys:
   - `OPENROUTER_API_KEY` for script generation
   - `REPLICATE_API_TOKEN` for video generation

4. Run the development server:
   ```bash
   npm run dev
   ```

5. Open [http://localhost:8000](http://localhost:8000) in your browser

## How It Works

1. **Enter Your Topic**: Provide a topic for your YouTube video
2. **Generate Script**: AI creates a compelling script for your video content
3. **Create Video**: Transform your script into a professional video
4. **Download & Share**: Download your video and upload to YouTube

## API Integration

This application integrates with:

- **OpenRouter API**: For AI script generation using Claude
- **Replicate API**: For AI video generation using google/veo-3

## Project Structure

```
src/
├── app/                 # Next.js app directory
│   ├── api/             # API routes
│   ├── page.tsx         # Main page
│   ├── layout.tsx       # Root layout
│   └── globals.css      # Global styles
├── components/          # React components
│   └── video-generator.tsx # Main video generator component
└── lib/                # Utility functions
```

## Customization

### Styling
The application uses Tailwind CSS for styling. You can customize the theme in `src/app/globals.css`.

### Components
UI components are built with shadcn/ui and can be found in `src/components/ui/`.

## Deployment

To deploy this application, you can use platforms like:

- Vercel
- Netlify
- AWS Amplify

Make sure to set your environment variables in your deployment environment.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.
