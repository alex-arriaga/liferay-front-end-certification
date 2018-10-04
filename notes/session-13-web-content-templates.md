# Session 13. Web Content Templates

How the web content can be displayed on a page.

We can use Clay and its components to make our templates easier to maintain.

Widgets can be embedded into templates.

We can set preferences for portlets in our templates.

```
<#assign VOID = freeMarkerPortletPreferences.setValue("view", "exampleView") />
```

We don't want to display anything, that's why we use `VOID`.


- Template reference structures with variables.
- Templates inherit global SCSS and Clay components from the theme.
- Generic Templates are stand-alone templates used to include reusable code.
