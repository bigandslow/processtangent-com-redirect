# processtangent-com-redirect

`CNAME` sets the GitHub Pages custom domain on the public mirror, `bigandslow/processtangent-com-redirect`. `mirror.yml` force-pushes `main` there, so a change to `CNAME` here changes the live Pages setting.

The custom domain is `www.processtangent.com`, not the apex. With the apex as the custom domain, Pages kept reusing an apex-only certificate, so `www` never got one. With `www` as the custom domain, Pages issues one certificate for both names and redirects the apex to `www`.
