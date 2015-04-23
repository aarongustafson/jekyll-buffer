# Post to Buffer From Jekyll

This generator send posts for Buffer. To work, this script requires a `BUFFER_ACCESS_TOKEN` environment variable and at least one of the following environment variables:

*  `BUFFER_TWITTER_PROFILE`
*  `BUFFER_FACEBOOK_PROFILE`
*  `BUFFER_LINKEDIN_PROFILE`

By default, Twitter gets sent the post title & URL. Facebook and LinkedIn get the YAML "description" or the post excerpt (as a fallback) plus the link. You can customize each with the following front-matter:

* `twitter_text` - This will be truncated to 117 characters to make room for the URL
* `facebook_text`
* `linkedin_text`

## Todo

* Allow selective posting by setting any of the front matter vars to false
* Google Plus (maybe when they allow posting to accounts)

## Limitations

* Only one of each account type allowed
