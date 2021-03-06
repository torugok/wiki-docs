---
title: Requirements
description: Prerequisites to install Wiki.js
published: true
date: 2019-12-08T17:56:25.175Z
tags: setup
---

# Server Requirements

Wiki.js runs on virtually any system where Node.js is supported.
This means it runs on **Linux**, **macOS**, **Windows** as well as container solutions such as **Docker / Kubernetes** and **Heroku**.

### CPU
Wiki.js runs perfectly fine on a single CPU core. However, **2 cores or more are recommended** to fully make use of the background workers.

### RAM
Linux systems should have **at least 1GB of RAM** to run Wiki.js. Windows and macOS systems usually require a bit more RAM.

### Storage
Storage requirements are based on the content you will enter. Wikis that consists almost exclusively of text are not likely to exceed a few megabytes. However, as soon as you upload images, videos or other files, you should plan your storage requirements accordingly.

At least 1 GB of storage dedicated to Wiki.js is recommended.

### Internet Access
Wiki.js will automatically check for new updates, languages, themes, etc. from time to time. You can [read more](/install/requirements/internet) about what data is downloaded.

An alternate method of [sideloading files](/install/sideload) is also available if your environment is cut from the internet.

# Domain

Wiki.js requires a dedicated sub-domain / domain *(e.g. wiki.example.com)*. You cannot map Wiki.js to a subfolder.

# Database

Wiki.js is compatible with any of the following database systems:

- MySQL **8.0 or later** *(MySQL **5.7.8** is partially supported, [read more](/install/requirements/mysql5))*
- MariaDB **10.2.7 or later**
- MS SQL Server **2012 or later**
- PostgreSQL **9.5 or later**
- SQLite **3.9 or later**

> :ok_hand: We highly recommend **PostgreSQL** for best performance and features. Development of Wiki.js is done using PostgreSQL and will therefore have better support.
{.is-success}

> :warning: SQLite is **not recommended** for mid to large deployments of Wiki.js.
{.is-warning}

You're expected to have installed one of these database engines already *(either locally, on another server or using a cloud service)*. Wiki.js requires an empty database and preferably a unique user / pass to connect to the database.

# Node.js

Node.js **10.12 or later** is required.
*Wiki.js will not run on older versions such as 8.x, 6.x or any version below 10.12!*

> :whale: **Using Docker?**
> 
> Skip this requirement! You don't need to install Node.js on your machine! It's included in the Docker image already.
{.is-info}

> :cloud: **Web Server**
>
> Wiki.js doesn't need any actual web server (such as nginx or Apache). However, you might need to put a reverse proxy in front of Wiki.js if you require advanced network / DNS configuration.
{.is-warning}

# Supported Browsers

The following browsers are supported:

- Google Chrome (including Android version)
- Mozilla Firefox
- Microsoft Edge
- Apple Safari (including iOS version)

Note that only the latest stable version of these browsers are supported. All browsers updates automatically in the background.

> There's limited compatibility with **IE11**. Users will be able to read content but not perform any editing action or use interactive features.
{.is-info}

![](https://a.icons8.com/ViUXyjOj/f4tFww/svg.svg){.align-abstopright}