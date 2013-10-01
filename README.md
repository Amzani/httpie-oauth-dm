httpie-oauth-dm
===============

Dailymotion OAuth2 plugins for [httpie](https://github.com/jkbr/httpie) 
```bash
$ pip install git+http://github.com/akhenakh/httpie-oauth-dm.git?#egg=httpie_oauth_dm
```
Usage
-----
```bash
$ export API_KEY=myapikey
$ export API_SECRET=myapisecret
$ http --auth-type=oauth2DM --auth=username:password GET https://api.dailymotion.com/me 
```
You can also use HTTPie sessions.
```bash
 # Create session
 $ http --session=dm --auth-type=oauth2DM --auth=username:password GET https://api.dailymotion.com/me
    
 # Re-use auth
 $ http --session=dm GET https://api.dailymotion.com/me
```

TODO
----
httpie oauth plugins API does not permit yet to deal with token refresh
