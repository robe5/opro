## 0.3.3

- [#8] Fix Doc urls (@robe5)

## 0.3.2

- Attempt to find user based on params[:username] from client in devise default find_user_for_auth

## 0.3.1

- [#7] Bugfix: Verify access_token, refresh_token, and code are unique before attempting to save (@twinge)

## 0.3.0

- Properly set attr_accessible for those apps that are requiring all attributes to be whitelisted.
- Allow access_token to be passed in header `curl -H "Authorization: token iAmAOaUthToken" http://localhost:3000`
- [#6] Implement Bearer scheme curl -H "Authorization: Bearer iAmAOaUthToken" http://localhost:3000
- Default `config.password_exchange_enabled' to true
- Allow multiple `find_user_for_auth` calls in setup to allow custom finders for facebook, etc.
- You can now rate limit incoming client applications.
- Allow clients to mitigate security threat (http://homakov.blogspot.com/2012/07/saferweb-most-common-oauth2.html)

## 0.2.0

- Allow password exchange for access_token using `config.password_exchange_enabled = true`

## 0.1.0

- Refresh Token Support
- Scoped permissions support
- Docs, Test, and ClientApp controllers can be skipped or over-ridden

## 0.0.1

- Initial Release