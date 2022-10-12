# Purpose
Provide a sanitized copy of the PDF version of "The SAFe Delusion: Information for decision-makers considering the SAFe framework".

## What's Here
A potentially unsafe PDF from a well-known member of the agile community was recently shared on LinkedIn. This was likely done in good faith, but may create a security risk for anyone who clicks on the PDF referenced in the link.

In a [deeply-nested comment][comment], there was a link to a web page that provided some opposing viewpoints on the SAFe framework. The page also had a link to a PDF version of the page's contents that appears potentially unsafe and exhibits a number of malware-like characteristics. This repository provides a sanitized version of that PDF.

Since the content of the page and the PDF are useful to the agile community, this repository was created to provide [a safer version of the PDF provided in the original link][sanitized_file]. See "The Problematic PDF File" section below for more details.

---

# Copyrights
## This README File
Copyright © 2022 CodeGnome Consulting, LTD

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">This README file</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/CodeGnome/information-for-decision-makers-considering-the-safe-framework-sanitized.git" property="cc:attributionName" rel="cc:attributionURL">CodeGnome Consulting, LTD</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

## Source Web Sites and PDF
- The copyright for the `safedelusion.com` web page and presumably the PDF generated from it are attributed as:

    > Copyright © naked Agility Ltd 2022

- The Google Doc version at `https://bit.ly/SAFe4DecisionMakers` is described as open source in the copyright line of the above-referenced web page, but no specific open source license is defined on the page or in the Google Doc. Please contact the copyright holder of that document with any questions about its licensing.

---

# Disclaimers
## Disclaimer of Copyright to Original PDF
The authors of this README and the sanitized PDF make no claims to copyright of any content outside of the README itself. The contents of the PDF were sanitized for community safety by an open source tool, and are in no way intended as a derivative work.

## Disclaimer of Warranty
THERE IS NO WARRANTY FOR THE CONTENTS OF THIS REPOSITORY, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE CONTENTS "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE CONTENTS IS WITH YOU. SHOULD THE CONTENTS PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.

### Limitation of Liability
IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE CONTENTS OF THIS REPOSITORY AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE CONTENTS (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE CONTENTS TO OPERATE WITH ANY OTHER PROGRAMS OR SERVICES), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.

---

# The Problematic PDF File
The PDF file was originally found within the web page at:

```text
http://safedelusion.com/wp-content/uploads/sites/2/2022/10/Information-for-decision-makers-considering-the-SAFe-framework.pdf
```

and retrieved at 2022-10-11T16:37:10-04:00. At that time, it showed a number of potentially-unsafe [behavioral results][behavioral_results] when run inside various VirusTotal sandboxes. These results included 8 Mitre ATT&CK Tactics And Techniques. Several of the findings were marked as possible spear-phishing links, privilege escalation attempts, and defense evasion techniques. Other issues were noted as well.

Please refer to the behavioral results document linked above for a full list of identified issues.

## A Sanitized Version of the PDF
A [safe(er) version of the original PDF][sanitized_file] was made using the MIT-licensed [DangerZone][dangerzone] tool. Please note that in order to preserve the searchable text layer of the PDF file, DangerZone also preserved a number of `bit.ly` links that all seem to resolve to a Google Doc at:

```text
https://docs.google.com/document/d/1EdkoKpURZREBOmArg4aopWTzOhvEPfCgTD-aLNMSTgg
```

Please use your own discretion regarding the safety of clicking through obfuscated trackers and link shorteners like `bit.ly`, as well as applications that run in your browser such as Google Docs or PDF viewers.

### Caveats: Sanitized PDF
The DangerZone-processed copy of the PDF is included in this repository for your (relatively) safer reading, should you be interested in using a PDF reader instead of the web site. Pragmatically, the content of the PDF appears to be a slightly reformatted version of the original [web page contents][web_page_url] that has been converted to the Portable Document Format.

### Caveats: Original Web Site
The web page itself triggered [no malware warnings when scanned as a web page][web_page_scan] at approximately the same time that the PDF was retrieved. That likely means any issues that are not false positives are limited to the PDF's contents rather than the contents of the web page. Of course, due diligence is always called for and *caveat emptor* applies even when the information is free.

---
Copyright &copy; 2022 CodeGnome Consulting, LTD

[behavioral_results]: https://www.virustotal.com/gui/file/a83b3ea8e9ec3700a404555daf1ca265fd1d8c4a793764ef32aa6a4699683113/behavior
[cc-by-sa-4.0]: https://creativecommons.org/licenses/by-sa/4.0/
[comment]: https://www.linkedin.com/feed/update/urn:li:activity:6984252750180057088?commentUrn=urn%3Ali%3Acomment%3A%28activity%3A6984252750180057088%2C6984354205650010112%29&replyUrn=urn%3Ali%3Acomment%3A%28activity%3A6984252750180057088%2C6984440183634944000%29
[dangerzone]: https://dangerzone.rocks/
[sanitized_file]: https://raw.githubusercontent.com/CodeGnome/information-for-decision-makers-considering-the-safe-framework-sanitized/main/information-for-decision-makers-considering-the-safe-framework-sanitized.pdf
[web_page_scan]: https://www.virustotal.com/gui/url/6cd46f8c623f36ffbef47d38a484173d8fb8d0b0978588e2a9badd218ab30440
[web_page_url]: https://safedelusion.com/
