# Cleanup Roadmap

Move completed items from `ROADMAP.md` to `ROADMAP_COMPLETE.md` and tidy up.

## Steps

1. Read both `ROADMAP.md` and `ROADMAP_COMPLETE.md`.
2. Identify all completed items in `ROADMAP.md` — these are items whose heading line contains `- [x]`.
3. For each completed item found:
   - The item consists of its `### - [x]` heading line **plus** all subsequent non-heading lines (body/description) up to the next `###` heading, `---` separator, or `##` section heading.
   - Append the item to the correct section in `ROADMAP_COMPLETE.md`. Match by section header (e.g. `## #A: Features: Text reading`). If the section doesn't exist yet in `ROADMAP_COMPLETE.md`, create it in the same relative order as in `ROADMAP.md`.
   - Remove the item (heading + body) from `ROADMAP.md`.
4. Clean up `ROADMAP.md`:
   - Remove any sections that are now empty (contain no `###` items). Keep the section if it still has at least one `### - [ ]` item.
   - Keep the header, the link to `ROADMAP_COMPLETE.md`, and the `Success Metrics` section regardless.
   - Update the `*Last updated:*` date at the bottom to today's date.
5. Clean up `ROADMAP_COMPLETE.md`:
   - Update the `*Completed items moved from ROADMAP.md*` date at the bottom to today's date.
6. Show a summary of what was moved (item IDs and titles).
7. If there are no completed items to move, say so and stop — don't make any edits.
