# PagePilot AI: Chrome's Smart Assistant 🚀

> Use AI in-place when reading content on web pages. No more tab switching, no more copy-pasting – access AI capabilities right where you're reading.

## Get started

- Download an extension from [Chrome Extension's web store](https://chromewebstore.google.com/detail/nanmbeollpecgnfbkjdeogajflidikgd)
- Or download an extension from the website [page-pilot.pro](https://www.page-pilot.pro/)

## Architecture

<img src="./assets/architecture.png" />

## Why PagePilot AI?

PagePilot AI chrome extension addresses a serious workflow inefficiency in web browsing: the context switching between websites and AI tools. Currently, users must copy text from their browser, switch tabs to access AI tools, paste the content, wait for processing, and switch back to continue browsing. This back-and-forth process breaks concentration and slows down Chrome users.

The PagePilot chrome extension integrates AI capabilities directly into Chrome's native right-click menu (or Context Menu), allowing users to process text instantly without leaving their current webpage. Whether you're a student researching papers, a professional analyzing content, or a regular user, the extension’s AI Actions eliminates tab switching keeping your focus on the current task.
The key problems we solve:

- Eliminated context switching between browser tabs and AI tools
- Saved time through instant text processing
- Improved focus by maintaining users in their current context
- Simplified access to AI tools during browsing

## Technical implementation. Chrome extension

### Project Structure

```
/
├── manifest.json            # Chrome extension manifest
├── popup.html              # Extension popup HTML
├── src/
│   ├── popup.tsx          # Popup entry point
│   ├── background.ts      # Background script
│   ├── contentScript.ts   # Content script
│   └── assets/            # Icons, logos
│   └── hooks/             # React hooks
│   ├── components/        # React UI components
│   ├── context/           # React context (storage)
│   ├── services/          # Service layer
│   ├── types/             # TypeScript types
│   └── utils/             # Utility functions
├── vite.config.ts         # Vite configuration
└── package.json
```

### Gemini Nano service

<img src="./assets/gem-nano-service-1.png" />

### Gemini Nano service. Model orchestration

<img src="./assets/gem-nano-service-2.png" />

### Gemini AI Request service

<img src="./assets/gem-service.png" />

## Technical implementation. Next.js app

### Gemini AI API (For Gemini Flash 8B, Flash and Pro models)

<img src="./assets/nextjs.png" />

## Examples

<img src="./assets/eg-5-1.png" width="700" />
<p>|</p>
<img src="./assets/eg-5-2.png" width="700" />

## Technologies Used

- Google Gemini Nano - Prompt API, Summarization API, Write API
- Google Gemini API - Flash 8B, Flash, Pro
- Chrome extensions API. Manifest v3.
- Frontend and Backend: Next.js, React, TypeScript, Vite, Material UI, Tailwind CSS
- Deployments: Vercel, Chrome Extension Web Store

## Contributors & Contact Details

👤 **Akezhan Rakishev**

- LinkedIn: [Akezhan Rakishev](https://www.linkedin.com/in/akezhan-rakishev-841505170/)
- Email: rakishev.akezhan@gmail.com
- Phone: +1 (628) 529-5586
