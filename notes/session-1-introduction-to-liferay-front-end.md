# Front-end Development in Liferay

## Introduction

There are three options for styling in Liferay:

Modules
	- Themes / layouts (global look and feel)
Templates (freemarker)
	Customization for content, assets and widgets
	- Web Content templates
	- ADTs
Fragments
	re-usable parts
	html/css/js for any aspect of the page (can be edited by marketing teams)


## Tools for building modules (themes / layouts)

- [Theme Builder Gradle plugin](https://dev.liferay.com/es/develop/reference/-/knowledge_base/7-1/theme-builder-gradle-plugin)
- [Liferay IDE](https://dev.liferay.com/es/develop/tutorials/-/knowledge_base/7-1/liferay-ide)
- [Blade CLI's theme template](https://dev.liferay.com/es/develop/tutorials/-/knowledge_base/7-1/blade-cli)
- [Liferay Theme Generator](https://dev.liferay.com/es/develop/tutorials/-/knowledge_base/7-0/themes-generator)
	- [Node.js](https://nodejs.org/en/)
	- [Yeoman](http://yeoman.io/)
	- [Gulp](https://gulpjs.com/) tasks

We will test our [Liferay Tomcat Bundle](https://www.liferay.com/downloads-community) (local development).

## Requirements
1. Download the [Java Development Kit 1.8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html).

**The bundle will NOT work with Java 9 or 10!**

2. Set your **JAVA_HOME** environment variable.

3. Get the bundle and assign your license (this will be provided by your company or you can request a trial in this page: )

4. Start your Tomcat

```
./catalina.sh run
```


## Starting with tooling
```
sudo npm install -g yo gulp
sudo npm install -g generator-liferay-theme
```
