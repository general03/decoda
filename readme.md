# Decoda v5.0.0-rc1 #

A lightweight lexical string parser for BBCode styled markup.

## Requirements ##

* PHP 5.3
* Composer

## Compatibility ##

* v3.x - PHP 5.2
* v4.x - PHP 5.3
* v5.x - PHP 5.3, Composer

## Contributors ##

* "Marten-Plain" emoticons by Mårten Lundin - http://adiumxtras.com/index.php?a=xtras&xtra_id=6920
* "HTML_BBCodeParser" by Seth Price - http://pear.php.net/package/HTML_BBCodeParser/

## Features ##

* Parses custom code to valid (X)HTML markup
* Setting to make links and emails auto-clickable
* Setting to use shorthand text for links and emails
* Provides Filters to parse markup and custom code
* Provides Hooks to execute callbacks during the parsing cycle
* Provides functionality to render complex markup using a template system
* Can censor offensive words
* Can convert smiley faces into images
* Basic support for localized messages
* Supports a wide range of tags
* Fixes incorrectly nested tags by removing the broken/unclosed tags
* Logs errors for validation

## Filters ##

The following filters and supported tags are available.

* Default: b, i, u, s, sup, sub, br, hr, abbr, time
* Block: align, float, hide, alert, note, div, spoiler, left, right, center, justify
* Code: code, var
* Email: email, mail
* Image: image, img
* List: list, olist, li
* Quote: quote
* Text: font, size, color, h1-h6
* Url: url, link
* Video: video, youtube, vimeo, veoh, liveleak, dailymotion, myspace, wegame, collegehumor

## Hooks ##

The following hooks are available.

* Censor: Censors all words found within config/censored.txt
* Clickable: Converts all non-tag wrapped URLs and emails into clickable links
* Emoticon: Converts all smilies found within config/emoticons.json into emoticon images

## Unsupported ##

* URLs that begin with www will not be converted (intentional)
* Certain videos are not supported as their embed code does not match the URL in the address bar

## Documentation ##

Thorough documentation can be found here: http://milesj.me/code/php/decoda

A Mootools textarea editor is also available: https://github.com/milesj/moo-decoda