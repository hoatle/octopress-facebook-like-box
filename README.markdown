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
$ cat _config_facebook_like_box.yml >> _config.yml # copy all settings from _config_facebook_like_box.yml to _config.yml
```
There could be some conflicts to resolve:


How to configure the settings
-----------------------------

- A custom aside box is introduced: `custom/asides/facebook_like_box.html` that could be included.

- Find at the end of `_config.yml` for possible settings. To enable this plugin,
`facebook_like_box_href` is required.


Authors and contributors
------------------------

- Hoat Le: https://github.com/hoatle

- Many thanks to https://github.com/geetotes/octopress-facebook-likebox for original work, I have
a different approach so I could not fork and make pull request.

License
-------

MIT license
