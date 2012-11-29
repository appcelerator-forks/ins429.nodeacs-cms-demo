###NODE.ACS (M)VC framework demo

Please do fill out your ACS app's oauth_key and oauth_secret_key on app.js.

    ACS.init('<OAUTH_KEY>', '<OAUTH_SECRET_KEY>');

To publish, modify package.json.

Read more about on Node.ACS, http://nodeacs.cloud.appcelerator.com/guides/quickstart.

#####Quick Start (CMS)

* Using express.js as web app framework
* Package.json,
* app.js
  * initialize ACS
  * setup express.js settings
  * choose view system for express.js: express-partials
* Routing: config.json
  * routing: determined which controller#function to use
  * filters
  * websocket(removed)
* Views
  * Assets, (public)/images, (public)/css, (public)/js
* Controllers
  * Methods and functions(actions)


Flash message:

a flash message something similar to flash on rails

    req.session.flash = {msg:"Please login first.",r:0};

msg: flash message, r: flag if flash has been read(1) or not(0)