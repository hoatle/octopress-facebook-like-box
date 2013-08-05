octopress-facebook-like-box
===========================

The Facebook like-box plugin for octopress from
https://developers.facebook.com/docs/reference/plugins/like-box/


How to install
--------------

``` bash
$ git remote add hoatle-octopress-facebook-like-box https://github.com/hoatle/octopress-facebook-like-box.git
$ git fetch hoatle-octopress-facebook-like-box
$ git merge hoatle-octopress-facebook-like-box/master
$ mv README.md README_facebook_like_box.md # rename README.md to avoid any conflict with other plugins with the same installation approach
$ cat source/_includes/facebook_like.html > source/_includes/facebook_like_backup.html # backup first before overwriting it
$ cat source/_includes/facebook_like_box.html > source/_includes/facebook_like.html # replace existing facebook_like.html by the one from octopress-facebook-like-box
$ cat _config_facebook_like_box.yml >> _config.yml # append all settings from _config_facebook_like_box.yml to _config.yml
```

After the installation, you could review all the changes to make sure there is nothing missing or
wrong.

How to configure the settings
-----------------------------

- A custom aside box is introduced: `custom/asides/facebook_like_box.html` that could be included.

- Find at the end of `_config.yml` for possible settings. To enable this plugin,
`facebook_like_box_href` is required.

Example
-------

This is the example done for http://blog.teracy.com

- add custom aside box to `default_asides`:

``` ruby
# To add custom asides, create files in /source/_includes/custom/asides/ and add them to the list like 'custom/asides/custom_aside_name.html'
default_asides: [custom/asides/facebook_like_box.html, asides/recent_posts.html, asides/github.html, asides/delicious.html, asides/pinboard.html, asides/googleplus.html]
```

- Set `facebook_like_box.href`:

``` ruby
# the URL of the Facebook Page for this Like Box. Note: After July 2013 migration, href should be
# an absolute URL.
facebook_like_box_href: https://www.facebook.com/teracy.official
```

Enjoy and happy blogging!

Authors and contributors
------------------------

- Hoat Le: https://github.com/hoatle

- Many thanks to https://github.com/geetotes/octopress-facebook-likebox for original work, I have
a different approach so I could not fork and make pull request.

License
-------

MIT license
