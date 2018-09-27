# Session 9. Themelets

Small, extendable and reusable pieces of code that can be implemented by the theme.

- CSS
- JavaScript
- Freemarker

They were introduced since **Liferay 6.2**.

## Creating a themelet

```
yo liferay-theme:themelet
```

They need to be visible via the NPM registry with `npm link` or installing them as global with `-g` flag.

Use npm link to make our themelet available 

```
cd /path/to/your/themelet
sudo npm link
```

Go to your theme and let's `extend` it.

```
cd /path/to/your/theme
gulp extend
gulp deploy
```

Since themelets are NPM modules, they need to be **installed** in the theme via `npm install` (production-ready).
