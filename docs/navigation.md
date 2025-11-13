# Build your navigation

Control the left-hand nav through the `nav` section of `mkdocs.yml`.

## Simple list
```yaml
nav:
  - Home: index.md
  - Getting Started: getting-started.md
  - API Reference: api-reference.md
```

## Grouped sections
```yaml
nav:
  - Home: index.md
  - About Template:
      - What this template does: template-overview.md
      - TechDocs + MkDocs: techdocs-and-mkdocs.md
  - Authoring:
      - Getting Started: getting-started.md
      - Authoring Guide: authoring.md
  - Reference:
      - API Reference: api-reference.md
```

## Nested pages
```yaml
nav:
  - Home: index.md
  - Guides:
      - Setup:
          - Prerequisites: guides/prereqs.md
          - Install: guides/install.md
      - Usage:
          - Basics: guides/usage/basics.md
          - Advanced: guides/usage/advanced.md
```

Tips:
- Keep titles concise and meaningful
- Order top-to-bottom by importance
- If a page is missing from nav, it won’t appear in the site even if the `.md` exists
