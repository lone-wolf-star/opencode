---
version: "1"
website_url: https://opencode.ai
media_path: /public
ssg_framework: astro
frontmatter_format: yaml
sitemap_url: https://opencode.ai/sitemap.xml
publishing_mode: direct_publish
i18n:
  enabled: true
  locales:
    - en
  default_locale: en
  prefix_default_locale: false
collections:
  - name: docs
    git_path: /src/content/docs/
    file_extension: .mdx
    filename_pattern: ""
    collection_type: grouped
    i18n:
      enabled: true
      strategy: path
    frontmatter_schema:
      - name: title
        type: title
        label: Title
      - name: description
        type: richtext
        label: Description
---

# GitCMS Configuration File

> [!WARNING]
> This file is managed by [GitCMS](https://gitcms.dev).
> Update configuration only from the GitCMS web app.
