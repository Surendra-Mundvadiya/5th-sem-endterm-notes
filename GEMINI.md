# Workspace Rules: End-Term Notes

## Document & Notes Formatting Rules
- **Prohibited Formats:** NEVER commit, save, or push notes or study documents in Microsoft Word or Office formats (`.docx`, `.doc`, etc.).
- **Mandatory Formats:** All notes, course summaries, and reading materials must be saved and pushed exclusively in **PDF (`.pdf`)** or **Markdown (`.md`)** formats. This ensures clean diff tracking, cross-platform readability, and persistent change history.

## Repository Synchronization Rules
- **Sync Protocol:** Whenever the user requests to "sync" (or "sync pull and push"), execute a complete synchronization workflow:
  1. Pull incoming remote changes: `git pull --rebase origin main` (or `git pull origin main`)
  2. Stage modified and new documents (excluding any ignored or office formats): `git add`
  3. Commit with a concise descriptive message
  4. Push local commits to remote: `git push origin main`
