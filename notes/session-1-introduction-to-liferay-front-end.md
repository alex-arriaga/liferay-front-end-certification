# Session #1. Introduction to Front-end in Liferay

## Introduction

There are three options for styling in Liferay:

 **1. Modules**
	- Themes / layouts (global look and feel)

**2. Templates (freemarker)**
	Customization for content, assets and widgets
	- Web Content templates
	- Application Display Templates (a. k. a. ADTs)

**3. Fragments**
	- Re-usable parts
	- HTML / CSS / JavaScript for customizing any aspect of the page (can be edited by marketing teams)


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

3. Get the bundle and your license (this license should be provided by your company or [you can request a trial in this page](https://web.liferay.com/sign-in?p_p_id=58&p_p_lifecycle=0&p_p_state=maximized&p_p_mode=view&_58_struts_action=%2Flogin%2Fcreate_account_trial&_58_redirect=%2Fc%2Fportal%2Fregister_trial_license%3Fredirect%3D%2Fdigital-experience-platform%2F30-day-trial)).
Once you have the bundle, decompress it in any folder in your computer where you have access and enter to it using your terminal.

The license is usually sent by email (the email you registered for the trial period).

```
cd /path/to/my/bundle/

# e. g.
cd /Users/alex/Sites/bin/liferay/bundles/liferay-dxp-digital-enterprise-7.1-m1
```

4. Start your Tomcat

```
# Enter to your Tomcat's bin folder
cd /Users/alex/Sites/bin/liferay/bundles/liferay-dxp-digital-enterprise-7.1-m1/tomcat-9.0.6/bin

# You can use two options to start Tomcat with Liferay
# 1) Using catalina.sh; this option will start watching the logs, but you cannot close the terminal (or the process will end)

./catalina.sh run
sh startup.sh

# 2) Using startup.sh; this will run the start process and there is no need to keep the terminal open

./startup.sh
sh startup.sh

# 2.1) To see the logs with this second option use:
# I am assuming you are in the 'tomcat-9.0.6/bin' directory

tail -f ../logs/catalina.out
```


## Starting with tooling

Let's install Yeoman, Gulp and the Liferay Theme generator as global NPM packages:

If you are in a UNIX-like operating system, then use **"sudo"** to authorize the process to install our packages.

```
sudo npm install -g yo gulp
sudo npm install -g generator-liferay-theme
```
