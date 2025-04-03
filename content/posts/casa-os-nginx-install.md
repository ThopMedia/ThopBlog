---
title: "Install Nginx Proxy Manager on Docker & CasaOS"
date: 2025-03-21
draft: true
author: "Nikhil Jayammagari"
avatar: "/img/nikhil.png"
cover: "https://i.postimg.cc/d3Lw9ZLK/Untitled-2.webp"
categories:
  - installation
tags:
  - casaos
  - nginx proxy
  - proxy
  - ssl
  - homelab
summary: Install Nginx Proxy Manager on Docker to easily manage reverse proxies with a web-based UI. Simplify SSL, domain routing.
---

**Getting Started**  
Install [CasaOS](https://blog.thopmedia.com/posts/casa-os-install/) and access the web UI by typing the IP address of the CasaOS server into your browser.

![nginx](https://i0.wp.com/kurisucode.com/wp-content/uploads/2023/05/Screenshot-2023-05-21-at-12.16.58-PM-min.png?resize=1024%2C653&ssl=1)

Log in with your username and password.

![nginx](https://i0.wp.com/kurisucode.com/wp-content/uploads/2023/05/Screenshot-2023-05-21-at-12.27.42-PM-min.png?resize=1024%2C653&ssl=1)

After creating your account, you’ll see the dashboard. Now, let's change the web UI port. By default, it's port 80, but we need ports 80 and 443 for NPM. So, change it to 8000. Click the settings button in the top-left.

![nginx](https://i0.wp.com/kurisucode.com/wp-content/uploads/2023/05/Screenshot-2023-05-21-at-12.27.54-PM-min.png?resize=1024%2C653&ssl=1)

Click “change” next to WebUI port and set it to 8000. After saving, the page will refresh, and you’ll need to log in again to access the dashboard.

Next, let’s install Nginx Proxy Manager. Click the App Store icon to find quick install options.

![nginx](https://i0.wp.com/kurisucode.com/wp-content/uploads/2023/05/Screenshot-2023-05-21-at-12.28.32-PM-min.png?resize=1024%2C653&ssl=1)

Scroll down to find Nginx Proxy Manager and click it.

![nginx](https://i0.wp.com/kurisucode.com/wp-content/uploads/2023/05/Screenshot-2023-05-21-at-12.28.43-PM-min.png?resize=1024%2C653&ssl=1)

Click "Install." Review the default configurations, then click “Ok” to start the installation.

![nginx](https://i0.wp.com/kurisucode.com/wp-content/uploads/2023/05/Screenshot-2023-05-21-at-12.28.52-PM-min.png?resize=1024%2C653&ssl=1)

After installation, the NPM icon will appear on your dashboard!

![nginx](https://i0.wp.com/kurisucode.com/wp-content/uploads/2023/05/Screenshot-2023-05-21-at-12.31.24-PM-min.png?resize=1024%2C653&ssl=1)

Give it a moment to finish installing, then click the NPM icon to open it in a new tab.

![nginx](https://i0.wp.com/kurisucode.com/wp-content/uploads/2023/05/Screenshot-2023-05-21-at-12.51.30-PM.png?resize=1024%2C653&ssl=1)

Log in using the credentials from the initial installation:

- `admin@example.com`  
- `changeme`

![nginx](https://i0.wp.com/kurisucode.com/wp-content/uploads/2023/05/Screenshot-2023-05-21-at-12.51.38-PM.png?resize=1024%2C653&ssl=1)

Enter your name, nickname, and email. Then, change the password to something strong.

![nginx](https://i0.wp.com/kurisucode.com/wp-content/uploads/2023/05/Screenshot-2023-05-21-at-12.52.57-PM.png?resize=1024%2C653&ssl=1)

Now you're ready to use Nginx Proxy Manager.
