 Screen Recording with Mux + Next.js

A lightweight Next.js app for uploading, processing and summarizing videos with Mux (video + AI features), built while learning from the freeCodeCamp YouTube tutorial.

 🚀 Project Overview

This project:
- Uses `@mux/mux-node` for creating upload URLs and managing assets
- Uses `@mux/ai/workflows` to generate intelligent video summaries/tags
- Includes frontend routes for upload + video status + playback
- Demonstrates Mux workflow, captions extraction, and server actions in Next.js 16+

 📁 Repo structure

- app Next.js routes (page.tsx, dashboard, video/[id])
- action.ts server actions for Mux uploads and asset status
- components UI components: `MuxPlayerWrapper`, `ScreenRecorder`, etc.
- public static assets

 🛠️ Setup

1. Install:
   - `npm install` (or `pnpm`, `yarn`)
2. Add env vars:
   - `MUX_ACCESS_TOKEN`
   - `MUX_SECRET_KEY`
3. Run:
   - `npm run dev`
4. Open: [http://localhost:3000](http://localhost:3000)

 ✨ Key Features

- Generate Mux upload URL with `createUploadUrl()`
- Check upload -> asset conversion status
- Poll and show subtitle transcript text
- Generate summary + tags from `@mux/ai/workflows`
- List latest videos with playback link

 🧩 How this works

- `createUploadUrl` creates asset + upload target
- `getAssetidFromUploadId` maps upload -> asset -> playback ID
- `getAssetStatus` polls status + text captions from `.vtt`
- `generateVideoSummary` uses Mux AI to create summary/tags

 🧪 Run locally

- `npm run dev`
- `npm run build`
- `npm start`

 📝 Acknowledgements

Thanks to the freeCodeCamp YouTube channel for the learning path and inspiration.  
This project was built from their tutorial examples Next.js + Mux app.



