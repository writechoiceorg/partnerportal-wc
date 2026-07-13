# Sync Images from Source to Draft

Given two documentation files — a **source** (authoritative/live page) and a **target** (draft/new version) — this command:

1. Extracts all image URLs from both files
2. Matches images by their position/context (figure order and surrounding description)
3. Updates any outdated image URLs in the target to use the source's URLs
4. Flags any images that exist in the target but have no counterpart in the source
5. Reviews each figure caption and surrounding text to check it accurately describes what the screenshot shows

## Usage

```
/sync-images <source-file> <target-file>
```

**Example:**
```
/sync-images get-started/set-up-your-partner-program/how-to-add-partner.mdx draft-template/setup/how-add-partner.md
```

Both paths are relative to the project root.

---

## Steps to follow

### 1. Read both files

Read `$ARGUMENTS` split on whitespace — first token is SOURCE, second is TARGET. Resolve both as paths relative to the project root.

### 2. Extract and compare images

For each file, extract every image in order:
- The Intercom CDN **image path** (the part before `?expires=`) — this identifies the actual image
- The surrounding context: the heading it falls under, the alt text, and the caption line immediately after (lines starting with `*Figure`)

Build two lists (source images, target images) keeping the context alongside each URL.

### 3. Match images between source and target

Match by **section context** (same heading / same step), not by position alone. For each pair:

- If the path differs → the target has an outdated image; note which URL to use from source
- If the target has an image with no counterpart in source → flag it for manual review
- If the source has an image not present in target → flag it as potentially missing

### 4. Update the target file

For each mismatch found in step 3:
- Replace the full image URL in the target (path + query params) with the source's URL
- Do NOT change alt text or captions during this step

Report each replacement made: old path → new path.

### 5. Review text against images

For each image in the target (after updates), review the figure caption and the surrounding paragraph. Check:

- Does the caption accurately describe what the screenshot likely shows, given the step context?
- Does the surrounding text describe UI actions (button names, tab names, menu paths) that match what would appear in that screenshot?
- Are there any captions referencing UI elements that were updated elsewhere in the file (e.g., "Partners tab → Invite button" when Step 1 now says "Invite Partner under Partners menu")?

Report any caption or text inconsistencies found, with the specific line and a suggested correction. Apply the corrections directly to the file.

### 6. Final report

Output a summary:
- Images updated: list of old → new
- Images flagged for manual review (no source counterpart)
- Text/caption inconsistencies fixed
- Any remaining items that need a human to provide a new screenshot
