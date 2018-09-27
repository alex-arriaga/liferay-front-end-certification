# Session 10. Adding resources

We can include resources for example: layouts, templates in the theme

## Resources Importer

It creates a site template for creating new sites with predefined look-and-feel.

The `sitemap.json` allows developers to designate structures, etc. (defines de Site Template or Site Structure).

`assets.json` metadata (categories, tags) in our assets that are imported.

Some folders we can create are:

`WEB-INF/src/resources-importer/document_library/documents` can contain files
`WEB-INF/src/resources-importer/journal` can contain templates, structures, and content articles (journal articles)
`WEB-INF/src/resources-importer/templates` contain application display templates

Documentation about the Resource Importer is available in: [Importing Resources with a Theme](https://dev.liferay.com/es/develop/tutorials/-/knowledge_base/7-0/importing-resources-with-a-theme).

## Important!

The Resources Importer is going to be replaced by the **Site Initializer** in future Liferay versions.

## Embedding widgets

We can add widgets to the `portal_normal.ftl` using following tag libs:

- <@liferay_porlet["runtime"]
- <@liferay_journal["journal-article]
- <@liferay_ui["asset-display"] (className, classPK -type of asset-, template)

When using tag libs be aware they are **heavy** code, so use them carefully.

