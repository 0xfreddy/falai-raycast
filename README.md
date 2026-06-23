# fal.ai Raycast Extension

Generate media from fal.ai models directly in Raycast.

## Flow

1. Add your fal API key in the extension preferences.
2. Run **Create**.
3. Search or paste any fal endpoint ID, then open the generation form.
4. Fill the schema-derived fields. Unsupported or complex fields can be supplied in **Raw JSON overrides**.
5. Submit the request. The extension stores the request ID and opens the generated result once complete.
6. Run **Generated Assets** to refresh older queued jobs, copy URLs, open media, or browse your fal Assets library.

The extension uses fal's model search endpoint with `expand=openapi-3.0`, submits through the async queue, and stores request metadata in Raycast local storage so long generations can be retrieved later.
