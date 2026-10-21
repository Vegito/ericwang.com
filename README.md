# ericwang.com

GitHub Pages site for the bare domain. Visitors to ericwang.com and www.ericwang.com are forwarded to
https://resume.ericwang.com (index.html and 404.html both redirect). Two paths are served as-is for
the Eric Tesla app:

- `/.well-known/appspecific/com.tesla.3p.public-key.pem` - public half of the Tesla Fleet API key
  (private half stays in C:\Keys on the build machine, never in this repo).
- `/erictesla/callback.html` - OAuth redirect page that hands the login code to the app.

`.nojekyll` makes GitHub Pages serve the dot-folder. `CNAME` binds the custom domain.
