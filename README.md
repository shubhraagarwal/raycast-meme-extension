# Memes/GIFs

Effortlessly discover and share the funniest memes and trending GIFs directly from Tenor, right within Raycast! Instantly fetch a wide variety of Indian and global memes, search by keyword, and preview or copy GIFs to use in your work or chats. Perfect for anyone who loves bringing humor and viral content into their workflow with zero friction.

## Features

- **Direct GIF Clipboard Copying**: Copy actual GIF files (not just URLs) directly to your clipboard for seamless pasting
- **Auto-close on Copy**: Extension automatically closes after copying, returning you to your workflow
- **Instant Search**: Search and discover memes and GIFs with real-time results
- **Infinite Scroll**: Load more GIFs as you scroll through results
- **Modular Architecture**: Built with React, TypeScript, and custom hooks for maintainability
- **Powered by Tenor**: High-quality GIF database with millions of memes

## Setup (Raycast Store)

1. Install the extension from the Raycast Store
2. Open Raycast and run the "Memes/GIFs" command
3. Enter your Tenor API key when prompted
4. Start searching for memes and GIFs!

## Local Development Setup

### Prerequisites

- **macOS** (required for Raycast)
- **Node.js** (v16 or higher)
- **Raycast** (installed on your Mac)
- **Tenor API Key** (free from [Google Developers Console](https://developers.google.com/tenor))

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/shubhraagarwal/raycast-meme-extension.git
   cd raycast-meme-extension
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Get a Tenor API Key**
   - Visit [Google Developers Console](https://developers.google.com/tenor)
   - Create a new project and enable the Tenor API
   - Generate an API key

4. **Run the extension in development mode**
   ```bash
   npm run dev
   ```

5. **Configure API Key**
   - Open Raycast (⌘ + Space)
   - Search for "Memes/GIFs"
   - Enter your Tenor API key when prompted
   - Start using the extension!

### Available Scripts

- `npm run dev` - Run the extension in development mode
- `npm run build` - Build the extension for production
- `npm run lint` - Run linter
- `npm run fix-lint` - Fix linting issues automatically

### Project Structure

```
src/
├── meme.tsx                    # Main entry point
├── components/
│   ├── ApiKeySetupForm.tsx    # API key configuration UI
│   ├── GifGrid.tsx            # GIF display grid with actions
│   └── LoadingGrid.tsx        # Loading state component
├── hooks/
│   ├── useApiKey.ts           # API key management hook
│   └── useGifQueries.ts       # Tenor API data fetching
├── utils/
│   └── appleScript.ts         # Native clipboard integration
└── types.ts                    # TypeScript type definitions
```

## Technical Stack

- **TypeScript** - Type-safe development
- **React** - UI component library
- **Raycast API** - Extension framework
- **TanStack Query** - Data fetching and caching
- **AppleScript** - Native macOS clipboard integration
- **Tenor API** - GIF/meme content source
