---
layout: post
title: GoPanel, A Minimalist Server Management Panel Written In Go
---

I wanted to share a little bit about a side project I’ve been working on recently. It’s called **GoPanel**. It’s a minimalist server management panel designed for easily managing LEMP (Linux, Nginx, MySQL/MariaDB, PHP) stacks. I’ve been having a lot of fun building it and thought I’d give you a peek into what it does and where it’s headed.

### What is GoPanel?

GoPanel is a server management panel that I built using Go for the backend and Vue.js for the front end. The main idea was to create a simple and effective tool for managing LEMP stacks on Debian-based systems. If you’re familiar with server management, you know it can sometimes get pretty complex to set things up for your website, so I wanted to create something that makes the process a bit easier.

### What’s Inside?

<img width="750" src="https://github.com/user-attachments/assets/eb0f7f77-111c-4e47-a597-3b216c1b56e0">

Here’s a quick rundown of what GoPanel offers so far:

- **Single Binary Deployment:** The entire panel runs from a single binary file. Thanks to the Golang Embed FS library, all the files are packed into this one binary, making it easy to get started using the panel.

- **OTP-Only Authentication:** Instead of dealing with usernames and passwords, GoPanel only uses OTP (One-Time Password) for authentication. It’s a simple way to handle security without adding extra layers of complexity.

- **Nginx Configuration Management:** There’s a site management panel that works directly with Nginx configurations. This means you can manage your sites and their settings right from the panel, without having to dig into Nginx config files manually.

<img width="750" src="https://github.com/user-attachments/assets/d9a24f3d-56a4-4652-80ec-a6f72742f54f">

- **File Manager:** The built-in file manager lets you handle files on your server directly through the panel and easily fix the permissions for the web server.

<img width="750" src="https://github.com/user-attachments/assets/a2b44ddb-a1f4-481b-b843-061031578aef">

<img width="750" src="https://github.com/user-attachments/assets/62bc929c-fd6e-4a0a-9daa-f66707add3f4">

- **Extensible API:** GoPanel comes with an API that lets you extend its functionality and manage a lot of things on your server, including file management, system load info, and more to come. 

### What’s Yet to Come?

There are a few things on my to-do list for GoPanel, including:

- **Redirects Management:** I plan to add functionality for managing redirects, which should make site management even smoother.

- **Cron Management:** I’m working on adding cron job management to help with scheduling tasks.

- **Logs Access:** Having access to logs is important for troubleshooting, so I’ll be adding log management features soon.

- **Database Management and More:** Future updates will include database management, PHP engine management, a web terminal, and SSH access management. These additions will make GoPanel a more complete tool for server administration.

- **Support for Other Distros:** Right now, GoPanel supports Debian-based systems, but I’m hoping to extend compatibility to other Linux distributions in the future.

### Check It Out

If you’re curious and want to check out the project, you can find it on [GitHub](https://github.com/xaymup/GoPanel). It’s still a work in progress, and I’m always open to feedback or contributions. 

## Final Thoughts

Building GoPanel has been a fun and educational experience. It’s a hobby project, so I’m working on it as I find time, but I’m excited about where it’s headed. If you’re interested or have any thoughts to share, feel free to reach out.

