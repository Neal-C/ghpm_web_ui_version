# Documentation

## Resources

- [Github API docs](https://docs.github.com/en/rest)

## How stuff on github actually works

- https://trufflesecurity.com/blog/anyone-can-access-deleted-and-private-repo-data-github

## Oauth2 flow

### Oauth2 with CSRF Protection with "state" parameter

the state parameter is supported by github and will be used to prevent CSRF attacks.

Backend checks the state parameter and if it is not the same as the one stored, it will return an error.

Frontend checks the state parameter and if it is not the same as the one stored, it will stop the authentication flow.