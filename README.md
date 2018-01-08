This is a fork from https://github.com/julianlam/nodebb-plugin-sso-oauth

# Difference from nodebb-plugin-sso-oauth
All settings are being set in a config file (`nodebb/sso-config.json`). It also parses the id from the jwt token (field name needs to be set in `sso-config.json`), so unless you're using jwt you need to update the behaviour of the `OAuth.getUidFromToken` in `library.js:230`.

## How to Adapt

1. Copy the sample `sso-config-sample.json` into `nodebb/sso-config.json`.
1. Update `sso-config.json` accordingly.
1. Activate this plugin from the plugins page
1. Restart your NodeBB
1. Let NodeBB take care of the rest

## Trouble?

Find us on [the community forums](http://community.nodebb.org)!