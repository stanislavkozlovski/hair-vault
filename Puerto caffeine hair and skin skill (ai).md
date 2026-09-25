---
provenance: ai-generated
status: unreviewed
reviewed_by_human: false
---

# Puerto caffeine hair and skin skill (ai)

## Pass 0: Problem or opportunity framing

### Who is the user, what do we know about their behavior, and how correct does the result need to be?

- **User:** Stan, researching hair loss and skin issues in the hair vault.
- **Their behavior:** Stan names one Puerto video already imported into `~/hair` and asks Codex to inspect its transcript and archived comments for firsthand reports.
- **Edge-case tolerance:** Stan does not accept missing even a rare relevant anecdote within the selected local import or falsely claiming complete coverage.

### What is the prevailing user problem or opportunity?

- **Problem or opportunity:** Stan cannot reliably find every firsthand report connecting ingested caffeine with hair or skin changes in a selected Puerto import, so useful anecdotes remain buried.

### What is the proposed solution, and why is it right for the user?

- **Solution:** Add a `SKILL.md` workflow that audits the selected local transcript and full comment archive for ingested coffee, tea, and caffeine without web search, with a script if needed to account for every record.
- **Why it fits the user:** It uses Puerto material already saved in the vault and produces source-linked findings Stan can check in Obsidian.

### How would you describe the end-to-end user experience?

- **End-to-end user experience:** Stan names an imported video, Codex checks its local transcript and comments, saves source-linked improvement, worsening, and no-change reports under hair, scalp, and general skin, and reports any coverage gap.

### What existing data, behavior, or integrations must keep working?

- **Legacy data:** Existing `04-Source-Links/Puerto/` snapshots, `02-Transcripts/` copies, and older anecdote notes that cite `/home/ops/puerto/downloads` remain readable and unchanged.
- **Legacy behavior:** The vault keeps source archives untouched and marks new AI-authored notes with provenance and review status.
- **Existing integrations:** The skill reads only imported hair-vault material, while `hair-vault` stores the skill, optional scripts, and design documents.
- **Compatibility tolerance:** Earlier notes remain intact, and the new workflow may add separate findings and coverage records for the selected import.

### Agent edge-case scan

| Edge case | What happens if ignored | What handling it adds | User decision |
|---|---|---|---|
| When Stan selects an import without a complete local comment archive, Codex cannot inspect every comment and reply. | Codex may present an incomplete list as exhaustive. | Codex checks the local archive status and record counts, then reports the missing material before claiming coverage. | UNDECIDED — HANDLE / IGNORE |
| When a commenter describes changed shedding without naming coffee or caffeine, a keyword prefilter skips the report. | Codex misses a relevant anecdote and overstates coverage. | Codex reviews every comment and its thread context and accounts for each archived record. | UNDECIDED — HANDLE / IGNORE |
| When the same comment appears in source JSON and copied Markdown, Codex encounters the anecdote twice. | Codex inflates counts and repeats the evidence. | Codex identifies findings by video and comment ID and links one source record. | UNDECIDED — HANDLE / IGNORE |
| When a speaker or commenter repeats another person's experience, Codex encounters a secondhand claim. | Codex misattributes the outcome to a firsthand witness. | Codex separates firsthand, secondhand, and general claims while preserving the relevant wording. | UNDECIDED — HANDLE / IGNORE |
| When an archived comment mentions topical caffeine while Stan is asking about ingested coffee, tea, or caffeine, Codex encounters another exposure route. | Codex mixes topical and ingested exposure in one category. | Codex retains the observation and labels the route separately. | UNDECIDED — HANDLE / IGNORE |
