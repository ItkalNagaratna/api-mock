# API Mock

![Deploy to GitHub Pages](https://github.com/ItkalNagaratna/api-mock/actions/workflows/deploy.yml/badge.svg)

A modern, intuitive tool to transform JSON data into usable code artifacts for your development workflow. Instantly generate TypeScript interfaces, Zod schemas, and MSW handlers from any JSON structure.

![AI Powered Mock Generation](./src/assets/dashboard_ai.png)

## 🚀 Features

- **🪄 AI-Powered JSON Generation**: Instantly create complex mock data structures using natural language prompts via the floating AI command bar.
- **🔐 Secure Gemini Integration**: Securely store your Google Gemini API key in local storage to unlock advanced generative capabilities.
- **⚡ Instant Code Generation**: Convert JSON to TypeScript interfaces, Zod schemas, and MSW handlers in real-time.
- **🌳 Visual Tree View**: Explore your JSON structure with a clean, interactive tree representation.
- **🎲 Smart Data Randomization**: Generate mock data variations while preserving the original JSON structure.
- **🛠️ Developer First DX**: 
  - Powered by Monaco Editor (the core of VS Code).
  - One-click copy and file downloads.
  - Built-in JSON formatting and validation.
- **🌈 Glassmorphism UI**: A beautiful, modern interface with smooth animations and responsive design.

### 🧪 Advanced AI Configuration
![AI Configuration Mode](./src/assets/ai_config.png)
Simply enter your Gemini API key in the configuration modal to enable the AI features. Your key is only used to communicate with the Google Generative AI API and never leaves your browser.

## 🛠️ Built With

- **React 19** - Modern UI components and hooks.
- **TypeScript** - Type-safe development.
- **Vite 8** - Lightning-fast build and dev server.
- **Tailwind CSS 4** - Modern styling.
- **Monaco Editor** - Robust code editing experience.
- **Lucide React** - Beautifully simple icons.
- **Vitest** - Unit testing for core logic.

## 🏁 Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn

### Installation

1. Clone the repository:
   ```bash
    git clone https://github.com/ItkalNagaratna/api-mock.git
    cd api-mock
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

### Running Tests

To ensure everything is working correctly, run the unit tests:
```bash
npm test
```

## 🧩 Reusing the Logic

If you want to use the generation engine in your own projects without the full UI, you can easily copy the core utilities:

1.  **Copy Utils**: Grab the `src/utils/` directory. It contains `typeGenerator.ts` and `mockGenerator.ts`.
2.  **Usage Example**:
    ```typescript
    import { generateTypeScript } from './utils/typeGenerator';
    
    const json = { id: 1, name: "Test" };
    const tsCode = generateTypeScript(json, "MyResponse");
    console.log(tsCode);
    ```

*Note: If you'd like to see this as a standalone NPM package, feel free to open an issue!*

## 📖 Usage

1. **Input**: Paste your JSON response into the left panel.
2. **Review**: Use the middle panel to visually inspect the data structure.
3. **Customize**: Click the settings icon in the bottom right to adjust the generated names.
4. **Export**: Copy the generated code from the right panel or download it as a `.ts` file.
5. **Randomize**: Use the "Randomize" button in the header to generate mock data for testing edge cases.

## 🧪 Development Workflow Improvements

We take DX seriously. Recent improvements include:
- **Unit Testing**: Core logic is covered by Vitest to prevent regressions.
- **Modular Utilities**: Decoupled generators for better maintainability.
- **Enhanced Monaco Integration**: Improved JSON validation and formatting.
- **Automated Downloads**: Easily export artifacts directly to your project.

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---
Crafted with ❤️ for developers who hate manual type definitions.
