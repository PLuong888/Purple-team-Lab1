# Publish this portfolio to GitHub

This package is prepared for repository `PLuong888/Purple-team-Lab`. It has **not** been uploaded or pushed automatically.

## Upload through GitHub Desktop (Windows)

1. Clone `https://github.com/PLuong888/Purple-team-Lab1` with GitHub Desktop.
2. Extract the ZIP and copy the **contents** of `Purple-Team-Home-Lab-GitHub-Ready/` into the cloned repository folder, replacing its existing `README.md` if you want the new portfolio overview.
3. Verify that `README.md`, `docs/`, `screenshots/`, and `diagrams/` are all at the repository root.
4. Review `EVIDENCE_STATUS.md` and confirm no unredacted secret or private information remains.
5. Commit with a message such as `Add Word reports and organised lab evidence`.
6. Select **Push origin**.

## Upload with Git (PowerShell)

```powershell
git clone https://github.com/PLuong888/Purple-team-Lab1.git
cd Purple-team-Lab1
# Copy the extracted portfolio folder CONTENTS into this folder.
git status
git add .
git commit -m "Add Word reports and organised lab evidence"
git push origin main
```

Do **not** publish the raw original PDF, terminal password output, `.vdi` / `.vmdk` disk images, host private SSH keys, or source backups. These are intentionally excluded from the package.

## Viewing the reports

GitHub renders the root `README.md` normally. The `docs/*.docx` files are Word documents that viewers will usually download rather than read inline in GitHub. Screenshots are both embedded in Word and separately filed by week under `screenshots/`.

## Known limitations

- This package contains 13 reports converted to DOCX, reflecting the reports previously prepared in this conversation.
- It does not include the three earlier day-level reports authored outside this package (Days 01–02, 03–04, and 07) or a verified `local_rules.xml`, because their original files have not been supplied.
- Some earlier checklist screenshots are not recoverable from the available PDF. They are listed in `EVIDENCE_STATUS.md` rather than fabricated.
- The Wazuh administrator password appeared in the supplied PDF; the public image has been redacted, but the original password **must be rotated** if still active.
