# SEO optimizations for Silverstripe

- Real-time in-cms SEO page analysis with tips & score (no need to save/refresh)
- May contain parts of Yoast's WP SEO plugin
- Contains parts of Bart's/30's Silverstripe SEO plugin
- Re-adds the 'MetaTitle' field that was removed in SilverStripe 3.1 (thanks to Loz Calver)

## Maintainer Contacts

* Bart van Irsel (Nickname: hubertusanton)
* [Dertig Media](http://www.30.nl)
* Michael van Schaik (Nickname: micschk)
* [Restruct](http://restruct.nl)

##Notes:##

Template tags:
- $SeoBreadcrumbs -> added microdata for breadcrumbs in SERP

Todo:
- resolve conflicts / update de.yml & es.yml

##Contributing:##

Pull requests are welcome for improvements & translations.

##Installation:##
Simply clone or download this repository, copy it into your SilverStripe installation folder, then run `dev/build`.

###Composer:###

```
composer require: "micschk/silverstripe-seo": "dev-master"
```

## Requirements

* SilverStripe 3.1

## Documentation

This modules helps the administrator of the Silverstripe website in getting good results in search engines.
A rating of the SEO of the current page helps the website editor creating good content around a subject
of the page which can be defined using a google suggest field.

The fields for meta data in pages will be moved to a SEO part by this module.
This is done for giving a realtime preview on the google search result of the page. 

In seo.yml config file you can specify which classes will NOT use the module. 
By default every class extending Page will use the SEO module.
Caution: The new master branch is not compatible with old releases see [this pull request](https://github.com/hubertusanton/silverstripe-seo/pull/10) from [jonom](https://github.com/jonom) (thanks!).
Please use tag 1.1 in old sites with the old config and tag 2.0 for new projects, but updating to 2.0 will also fix google suggest and
has some other fixes.


## Screenshots

![ScreenShot](https://raw.github.com/hubertusanton/silverstripe-seo/master/images/screen2.png)
![ScreenShot](https://raw.github.com/hubertusanton/silverstripe-seo/master/images/screen3.png)

## Installation
Place the module dir in your website root and run /dev/build?flush=all

## TODO's for next versions

- [ ] Check img tags for title and alt tags
- [x] Option to set social networking title and images for sharing of page on facebook and google plus
- [ ] Create a google webmaster code config 
- [ ] Only check for outgoing links in content ommit links within site
- [ ] Translations to other languages
- [ ] Check for page subject usage in other pages 
- [ ] Check how many times the page subject has been used and give feedback to user
- [x] (Re)Calculate SEO Score in realtime with javascript without need to save first
- [x] Put html in cms defined in methods in template files
- [ ] Check extra added db fields/ many_many DataObjects for SEO score and make this configurable

## License

This module is published under BSD 2-clause license, although these are not in the actual classes, the license does apply:

http://www.opensource.org/licenses/BSD-2-Clause

Copyright (c) 2013, Bart van Irsel

All rights reserved.

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

