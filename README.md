NODE.ACS
(M)VC framework demo.

Routes:
  defined in config.json under routes array.
  { "path": "/login", "method": "get", "callback": "application#login" }
  path: url path.
  method: only works for get & post by default(I believe).
  callback: <controller>#<function>

  * to select all
  { "path": "*", "method": "get", "callback": "application#page_not_found" }

Flash message:
  a flash message something similar to flash on rails
  req.session.flash = {msg:"Please login first.",r:0};
  msg: flash message,
  r: flag if flash has been read(1) or not(0)

* Quick Start (CMS)
  -Using express.js as web app framework
  -Package.json,
  -app.js
    + initialize ACS
    + setup express.js settings
    + choose view system for express.js: express-partials
  -Routing: config.json
    + routing: determined which controller#function to use
    + filters
    + websocket
  -Views
    + Assets, (public)/images, (public)/css, (public)/js
    + 
  -Controllers
    + Methods and functions(actions)