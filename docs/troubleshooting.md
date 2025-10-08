# Troubleshooting

## My page doesn’t show up in the left nav
- Ensure the page is listed under `nav` in `mkdocs.yml`
- Check the file path and capitalization

## RHDH shows no documentation
- Confirm your entity has the annotation `backstage.io/techdocs-ref: dir:.`
- Verify `mkdocs.yml` exists at the repo root and `docs_dir` points to your docs directory
- Ask your RHDH admins if TechDocs is enabled for your instance

## Build failed in TechDocs
- Look at the TechDocs build logs for the entity
- Validate YAML syntax in `mkdocs.yml`
- Validate Markdown links (relative paths)

## mkdocs serve fails locally
- Ensure MkDocs and dependencies are installed
- Run with `--config-file mkdocs.yml` from repo root
- Check for tabs/spaces issues in YAML

## Images not rendering
- Use relative paths from the page location
- Keep images within the docs directory (e.g., `images/`)

## Edit this page link missing
- Set `repo_url` and `edit_uri` in `mkdocs.yml`
