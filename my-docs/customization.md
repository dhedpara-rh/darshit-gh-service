# Customize mkdocs.yml

The `mkdocs.yml` file controls your site. This template provides sensible defaults and the `techdocs-core` plugin.

## Basic settings

```yaml
site_name: 'darshit-gh-service Documentation'
site_description: 'Documentation for darshit-gh-service'
repo_url: https://github.com/dhedpara-rh/darshit-gh-service
edit_uri: edit/main/my-docs

# Where your Markdown lives
docs_dir: my-docs

plugins:
  - techdocs-core
```

- site_name: Title shown in the header
- repo_url: Enables repo links in the header
- edit_uri: Adds “Edit this page” links to docs
- docs_dir: The docs source directory (matches your MR input)

## Navigation (`nav`)
Define the left-hand navigation order and grouping.

```yaml
nav:
  - Home: index.md
  - About Template:
      - What this template does: template-overview.md
      - TechDocs + MkDocs: techdocs-and-mkdocs.md
  - Authoring:
      - Getting Started: getting-started.md
      - Authoring Guide: authoring.md
      - API Reference: api-reference.md
  - Customize:
      - Navigation: navigation.md
      - mkdocs.yml Customization: customization.md
  - Troubleshooting: troubleshooting.md
  - FAQ: faq.md
```

## Theme and appearance (optional)
You can enable themes like `mkdocs-material` if allowed by your platform.

```yaml
theme:
  name: material
  features:
    - navigation.tabs
    - content.code.copy
```

Add extra assets:

```yaml
extra_css:
  - styles/overrides.css
extra_javascript:
  - js/extra.js
```

## Plugins (advanced)
You can add MkDocs plugins to extend functionality. TechDocs requires `techdocs-core`.

```yaml
plugins:
  - techdocs-core
  - search
  # - awesome-pages
  # - redirects
```

Coordinate with your RHDH admins before introducing new plugins/themes in shared environments.
