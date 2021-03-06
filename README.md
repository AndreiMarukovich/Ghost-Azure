# [Ghost (0.7.1)](https://github.com/TryGhost/Ghost) [![Deploy to Azure](http://azuredeploy.net/deploybutton.png)](https://azuredeploy.net/)

Want to install Ghost on Azure? Just click the 'Deploy to Azure' button and you're well on your way to have a Ghost Blog running within a minute or two. Made with :heart: for Ghost by Microsoft DX.

**Note: After deployment, Ghost will continue setup - resulting in your brand new website staying blank on the very first load. Just refresh, you'll see that everything worked well!**

#### Custom Domain
Directly after installation, Ghost will assume that your blog runs at `http://sitename.azurewebsites.net`. Should you switch to a custom domain, please inform Ghost about that change - you can do by setting the App Setting `websiteUrl` and restarting your website.

## Ghost
![Ghost Screenshot](https://cloud.githubusercontent.com/assets/120485/4828504/9e832764-5f80-11e4-8ac1-0332bcc67a35.png)

Ghost is a free, open, simple blogging platform that's available to anyone who wants to use it. Lovingly created and maintained by [John O'Nolan](http://twitter.com/JohnONolan) + [Hannah Wolfe](http://twitter.com/ErisDS) + an amazing group of [contributors](https://github.com/TryGhost/Ghost/contributors).

Visit the project's website at <http://ghost.org> &bull; docs on <http://support.ghost.org>.

## Running Locally

To run ghost locally run npm install then simply add websiteUrl, PORT, and NODE_ENV to your environment variables and run npm start. By default NODE_ENV will default to development, but the process that runs in azure runs with the value of production. If you decide to run NODE_ENV as production, you will probably want to turn off forceAdminSSL in config.js otherwise trying to access admin will default to redirecting you to https, and you won't have a valid SSL cert locally. The websiteUrl can be something as simple as `http://localhost` and the PORT variable should be the port you wish the instance to listen on.


## Copyright & License

Ghost is Copyright (c) 2013-2015 Ghost Foundation - Released under the [MIT license](LICENSE).
