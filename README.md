# fishcut

**AI agents draft shorts. You finish them.**

fishcut is a local shorts editor built for working with Claude Code and Codex. Give an agent a topic, develop a draft with a reusable template, then review and finish the video in the editor.

[Website](https://fishcut.nomadamas.org/) | [English website](https://fishcut.nomadamas.org/en/)

> **Development preview:** the features and videos below show the current development build. This public repository contains the project introduction; the source code and installation guide are being prepared for release.

## See it in action

[![Watch the fishcut editor demo: script, vertical preview, and layer timeline](https://fishcut.nomadamas.org/assets/shots/demo-edit-poster.webp)](https://fishcut.nomadamas.org/assets/shots/demo-edit.mp4)

**[Watch the editor demo](https://fishcut.nomadamas.org/assets/shots/demo-edit.mp4)** - a 34-second silent recording. Click the preview to open the MP4.

### Made with fishcut

Click a thumbnail to watch the full video with audio. These are finished shorts, separate from the editor recording above.

| A browser request, explained in Korean | Reverse Engineer Anything, explained in English |
|:---:|:---:|
| [<img src="https://fishcut.nomadamas.org/assets/shorts/browser-journey-ko.jpg" alt="Korean short explaining what happens when you type a website address into a browser" width="180">](https://fishcut.nomadamas.org/assets/shorts/browser-journey-ko-full.mp4) | [<img src="https://fishcut.nomadamas.org/assets/shorts/rea-reverse-engineer-en.jpg" alt="English short introducing Reverse Engineer Anything" width="180">](https://fishcut.nomadamas.org/assets/shorts/rea-reverse-engineer-en-full.mp4) |
| [Watch the full short - 1 min](https://fishcut.nomadamas.org/assets/shorts/browser-journey-ko-full.mp4) | [Watch the full short - 41 sec](https://fishcut.nomadamas.org/assets/shorts/rea-reverse-engineer-en-full.mp4) |

More examples and editor screens are on the [website](https://fishcut.nomadamas.org/en/).

## The workflow

1. **Choose a topic and a visual template.** Ask Claude Code or Codex for a product demo, a list of tips, a comparison, or an explainer.
2. **Review the script, then build the draft.** The agent gathers sources and prepares narration, caption timing, visuals, motion, and audio. Paid voice generation requires a separate approval.
3. **Finish it in the local editor.** Adjust text, scene timing, media, sound effects, and BGM. Agent edits through the CLI appear in the open editor, so you can keep working on the same project.
4. **Render, review, and choose where it goes.** Export a vertical MP4, check the picture and sound, then review the destination and upload settings. Publishing requires your confirmation.

## In the current development build

- **Reusable templates.** Separate the visual layout from the script style. Start from a frame, reuse a saved tips template, or develop a new template from a reference.
- **A local visual editor.** Work with a vertical preview, script panel, media library, layer timeline, and audio controls. Document projects support draft comparison before saving and rendering.
- **Voice and caption timing.** Local narration supports voice cloning. A free M1 voice option and paid Typecast/ElevenLabs integrations are connected in development, with end-to-end generation validation still in progress. Korean is the default; supported styles also produce English shorts.
- **Motion and 3D explainers.** Combine screen recordings, images, captions, and graphics. FFmpeg and HyperFrames render the video; ManimGL supplies animated 3D diagrams.
- **Mobile preview guides.** Check captions and key visuals against approximate interface overlays and recommended safe zones for YouTube Shorts, Instagram Reels, and TikTok.
- **Versioned MP4 exports.** Keep finished renders outside the working project, with separate versions for revisions.
- **Channel planning and upload flows.** Save each channel's audience, tone, language, and publishing defaults. The editor includes YouTube uploads and scheduling, Instagram Reels publishing, and TikTok inbox drafts for completion in the TikTok app.

The native workflow targets **macOS on Apple Silicon**. A **Docker Compose** runtime is also being tested. Voice providers and publishing services need their own setup; provider validation and platform app reviews are still in progress.

## Visual templates

All frames target **9:16, 1080 × 1920** video. Choose the layout first; fishcut connects a matching script style automatically. You can also select another compatible style for the topic.

| Frame | Best suited to |
|---|---|
| `letterbox` | Product demos and commentary, with a fixed title, source footage, and captions on a dark background |
| `post-app` | Tips and lists presented as a community post, with a header, title, captions, and supporting media |
| `canvas` | Explainers with a light canvas, central cards, and motion graphics |
| `canvas-dark` | Comparisons, prices, large numbers, and charts on a dark canvas |
| `manim-dark` | Mathematical and technical explainers built around animated 3D diagrams |

Script styles cover demos, explainers, factual narration, post readings, tips, and stories with a twist. The layout and script style can be reused independently where their rendering requirements match.

## Public release status

This repository currently contains the project introduction. The codebase and setup instructions are being prepared for public release.

Active development continues in a separate development repository. Reviewed code and redistributable assets will be brought here after private project files, third-party reference material, credentials, and local run records are removed. Development will move to this repository as the project matures.

Built by [NomaDamas](https://github.com/NomaDamas).
