# Intake and Extraction Workflow

1. Run `patent-intake` to create `input-register.md` and `missing-inputs.md`.
2. Run `document-extractor` on each registered file.
3. Record extraction confidence: `high`, `medium`, `low`, or `failed`.
4. For images, record only visible observations and do not infer hidden text or components.
5. Handoff `document-summary.md`, `image-observations.md`, and all missing information to `invention-structurer`.
