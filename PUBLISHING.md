# Publishing checklist

Run through this list before a report goes into `reports/`.

## Before the commit

- [ ] Written client approval to publish. Keep the email or chat screenshot in the private Sanad Squad drive, never in this repo.
- [ ] Fix review finished. Every finding has a status: Fixed, Partially fixed, Acknowledged or Won't fix.
- [ ] Report states the audited commit hash and the fix-review commit hash.
- [ ] Client asked for redactions? Remove private repo URLs, client staff names, internal infrastructure and anything they flagged.
- [ ] PDF metadata cleared (Google Docs and Word write author names and edit history into the file).
  `exiftool -all= -overwrite_original report.pdf`
- [ ] File named `YYYY-MM-sanad-squad-<client>-<scope>.pdf`, lowercase, hyphens only.

## The commit

- [ ] PDF added under `reports/`.
- [ ] Row added to the top of the audit table in `README.md` with severity counts.
- [ ] Commit message: `report: <client> <scope>`.

## After the commit

- [ ] Post from the Sanad Squad account and @0xcastle_chain with the report link, scope and severity counts.
- [ ] Add the report to the portfolio page on sanadsquad.com.
- [ ] Update the client row in the CRM sheet (Deals tab, Notes column) with the report link.

## Folder rules

- `reports/` holds final audit reports only.
- `research/` holds write-ups, vulnerability research, CTF write-ups and advisories (Markdown or PDF).
- `talks/` holds slides and recordings links from workshops and lectures.
