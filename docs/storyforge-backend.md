# Storyforge — Backend Concept (Future Evolution)

**Status:** Internal backend idea. Not active code. Evolves with Dreamforge as software develops.

## Origin
Mixed from:
- **Dreamforge** (theme park software)
- **litlitfire-mordor** (book-to-visuals: PDF processing, OCR, image generation)

## Core Idea
Turn books, PDFs, or rough story ideas into theme-park-ready experiences.

1. **Ingest & Extract** (litlitfire side)
   - Upload a book, PDF, or story outline.
   - Run OCR and visual extraction to pull scenes, characters, settings, and key beats.
   - Build a structured scene graph: locations, moods, props, dialogue, pacing.

2. **Experience Generation** (Dreamforge side)
   - Convert extracted scenes into interactive rides, immersive zones, and story beats.
   - Output: ride scripts, zone layouts, sensory cues (sound, light, projection), guest flow, and safety notes.
   - Keep everything model-agnostic — any strong enough model can run the extraction and generation layers. No specific model baked in.

3. **Monetization Paths**
   - Charge per generated experience or themed pack.
   - License full park builds to venues, studios, or attractions.
   - Optional marketplace for creators to sell story-to-experience templates.

## Integration Notes
- Lives in the backend of Dreamforge.
- Reuses litlitfire-style document/OCR pipelines where useful.
- Designed so the same interface can later plug into stronger models without rewriting the core.

## Next Steps (when ready)
- Define the scene-graph schema.
- Prototype one book → one ride flow.
- Add a simple cost/estimate layer for generated experiences.
