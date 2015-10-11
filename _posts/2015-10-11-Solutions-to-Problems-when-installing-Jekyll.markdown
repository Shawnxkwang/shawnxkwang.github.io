---
layout: post
title:  "Solutions to Problems when installing Jekyll"
date:   2015-10-11 17:05:30
categories: Solutions
---

When installing Jekyll for Github Pages, I encounter a problem when trying to 

`Bundle install`

And I get a error message:

Fetching gem metadata from https://rubygems.org/............

Fetching version metadata from https://rubygems.org/...

Fetching dependency metadata from https://rubygems.org/..

Resolving dependencies...

Installing RedCloth 4.2.9 with native extensions

Gem::InstallError: The 'RedCloth' native gem requires installed build tools.

Please update your PATH to include build tools or download the DevKit
from '[http://rubyinstaller.org/downloads](http://rubyinstaller.org/downloads)' and follow the instructions
at '[http://github.com/oneclick/rubyinstaller/wiki/Development-Kit](http://github.com/oneclick/rubyinstaller/wiki/Development-Kit)'

An error occurred while installing RedCloth (4.2.9), and Bundler cannot continue.

Make sure that `gem install RedCloth -v '4.2.9'` succeeds before bundling.


So I download the DevKit and install it under C://DevKit
Then follow the instructions at '[http://github.com/oneclick/rubyinstaller/wiki/Development-Kit](http://github.com/oneclick/rubyinstaller/wiki/Development-Kit)'

Yay! 
But…wait…
Then I ran into another problem:

Gem::RemoteFetcher::FetchError: SSL_connect returned=1 errno=0 state=SSLv3 read
server certificate B: certificate verify failed (https://rubygems.org/gems/i18n-
0.7.0.gem)
An error occurred while installing i18n (0.7.0), and Bundler cannot continue.
Make sure that `gem install i18n -v '0.7.0'` succeeds before bundling.


I googled around, found a solution to deal with this problem:
[http://stackoverflow.com/questions/27262582/i-get-certificate-verify-failed-on-installing-bundler-for-ruby-on-rails-on-wi](http://stackoverflow.com/questions/27262582/i-get-certificate-verify-failed-on-installing-bundler-for-ruby-on-rails-on-wi "Google solution")

Hope this can help people with same problems :)
