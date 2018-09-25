# browsersync
## what is browsersync
Time-saving synchronised browser testing.
It’s wicked-fast and totally free.
 [browsersync官网](https://browsersync.io/)

## quick start
1. Install Node.js
Browsersync is a module for Node.js, a platform for fast network applications. There are convenient installers for MacOS, Windows and Linux.
2. Install Browsersync
The Node.js package manager (npm) is used to install Browsersync from a repository. Open a terminal window and run the following command:
```cmd
npm install -g browser-sync
```
You’re telling the package manager to download the Browsersync files and install them globally so they’re available to all your projects.
3. Start Browsersync
A basic use is to watch all CSS files in the css directory and update connected browsers if a change occurs. Navigate your terminal window to a project and run the appropriate command:
3.1 Static sites
If you’re only using .html files, you’ll need to use the server mode. Browsersync will start a mini-server and provide a URL to view your site.
```cmd
browser-sync start --server --files "css/*.css"
```
3.2 Dynamic sites
If you’re already running a local server with PHP or similar, you’ll need to use the proxy mode. Browsersync will wrap your vhost with a proxy URL to view your site.
```cmd
browser-sync start --proxy "myproject.dev" --files "css/*.css"
```
