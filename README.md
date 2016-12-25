# NodeBB SmartID SSO

NodeBB Plugin that allows users to login/register via SmartID (https://smartid.ee)

## Installation

Install plugin and its dependencies with NPM:
```bash
npm install git+ssh://git@bitbucket.org:smartid/nodebb-plugin-sso-smartid.git
cd node_modules/nodebb-plugin-sso-smartid
npm install
```

## Usage

1. Register your NodeBB forum with SmartID (https://id.smartid.ee/admin/clientlist)
  * The redirect URL should be: http(s)://myforum.com/auth/smartid/callback
    * (In other words, add `/auth/smartid/callback` to the URL of your forum)
2. Add your client ID and secret in the code (line 46 and 47 in `library.js`)
2. Activate this plugin from the plugins page
2. Restart your NodeBB
