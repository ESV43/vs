# AI Comic Creator

## Overview

The AI Comic Creator is a full-stack web application that allows users to generate comic books from a simple story input. By leveraging advanced AI technologies, the application parses the story, extracts characters and scenes, generates illustrations, and composes a high-quality comic in PDF format.

## Features

- **Story Input**: Users can input a story of up to 10,000 words without needing to manually segment scenes or tag elements.
- **AI Processing**: The application utilizes various APIs to analyze the story, generate character art, and create scene images.
- **Comic Generation**: Automatically assembles comic pages with dialogue bubbles and illustrations.
- **PDF Export**: Users can download the final comic as a high-resolution PDF.
- **Local Storage**: Supports saving and re-opening previous sessions.

## Tech Stack

- **Frontend**: Vite, TypeScript, Vanilla JavaScript, HTML5, Tailwind CSS
- **APIs**:
  - Gemini API for natural language understanding
  - Pollinations API for AI image generation
  - HuggingFace API for advanced image generation models
- **PDF Generation**: jsPDF / html2pdf

## Project Structure

```
ai-comic-creator
├── assets
│   └── pages
├── public
│   └── index.html
├── src
│   ├── api
│   │   ├── gemini.ts
│   │   ├── pollinations.ts
│   │   └── huggingface.ts
│   ├── components
│   │   ├── StoryInput.ts
│   │   ├── GeneratorStatus.ts
│   │   ├── ComicPageRenderer.ts
│   │   ├── DialogueOverlay.ts
│   │   └── PDFExport.ts
│   ├── utils
│   │   ├── promptBuilder.ts
│   │   ├── sceneParser.ts
│   │   ├── localStore.ts
│   │   └── speechBubblePlacer.ts
│   └── main.ts
├── comic_output.pdf
├── session_export.json
├── package.json
├── tsconfig.json
├── tailwind.config.js
└── vite.config.ts
```

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/ai-comic-creator.git
   ```
2. Navigate to the project directory:
   ```
   cd ai-comic-creator
   ```
3. Install dependencies:
   ```
   npm install
   ```
4. Start the development server:
   ```
   npm run dev
   ```

## Usage

1. Open the application in your browser.
2. Enter your story in the provided text area.
3. Click the "Generate Comic" button to start the comic creation process.
4. Once the comic is generated, you can preview the pages and download the final PDF.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any enhancements or bug fixes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.