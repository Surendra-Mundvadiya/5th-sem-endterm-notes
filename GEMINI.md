# Workspace Rules: End-Term Notes

## Document & Notes Formatting Rules
- **Prohibited Formats:** NEVER commit, save, or push notes or study documents in Microsoft Word or Office formats (`.docx`, `.doc`, etc.).
- **Automatic Deletion:** Immediately delete `.docx` source files after converting them to `.pdf`.
- **Mandatory Notes Format:** All subject notes must be saved and pushed exclusively in **PDF (`.pdf`)** format. Do not create `.md` files for notes (only `syllabus.md` remains for syllabus tracking).
- **No Backups:** Do not create pre-change or revert backups for this repository.

## Repository Synchronization Rules
- **Sync Protocol:** Whenever the user requests to "sync" (or "sync pull and push"), execute a complete synchronization workflow:
  1. Pull incoming remote changes: `git pull --rebase origin main` (or `git pull origin main`)
  2. Stage modified and new documents (excluding any ignored or office formats): `git add`
  3. Commit with a concise descriptive message
  4. Push local commits to remote: `git push origin main`
