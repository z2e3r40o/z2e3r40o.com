+++
title = "gpg encrypt user emails with rails"
date = "2020-10-03"
author = "z2e3r40o"
authorTwitter = "z2e3r40o" #do not include @
cover = ""
tags = ["programming"]
keywords = ["rails gpg mail-gpg"]
description = "Example rails 6 application, deployable to heroku, that sends email pgp encrypted with user provided public key. Emails sent using mailgun."
showFullContent = false
+++

While using kraken.com to do some basic crypto trading, I came across what I think is a great feature. If you go to your account settings, you will find that you can add a _PGP Public Key_. Once you add your public key, all emails containing sensitive information will be encrypted for that public key before being sent to you.

I wish more of the sites I use had this feature. Since I haven't implemented this behavior in any of the projects I've worked on, I wanted to put together an example to show myself it wasn't too difficult to do.

You can see the example project I put together here: https://github.com/z2e3r40o/rails-with-gpg

The following technologies were used to put this example together:

- [rails 6](https://rubyonrails.org/)
- [mail-gpg](https://github.com/jkraemer/mail-gpg)
- [devise 4](https://github.com/heartcombo/devise)
- [heroku](https://heroku.com)
- [mailgun](https://www.mailgun.com/)
    - Actually, I used: [mailgun on heroku](https://elements.heroku.com/addons/mailgun)

In practice any one of these can be different.

This [rails-with-gpg](https://github.com/z2e3r40o/rails-with-gpg) repository can be deployed to heroku by simply cloning the repository, updating the config, and deploying to a heroku dyno. The [README](https://github.com/z2e3r40o/rails-with-gpg/blob/main/README.md) provides more instructions.
