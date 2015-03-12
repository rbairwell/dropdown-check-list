### Description ###
**Dropdown Check List** is a javascript plugin based on the **jQuery** library that transforms a regular **select** html element into a dropdown checkbox list.

[![](http://dropdown-check-list.googlecode.com/svn/trunk/doc/demo.png)](http://dropdown-check-list.googlecode.com/svn/trunk/doc/demo.html)

### Warning ###
<font color='red'>DDCL is only Minimally supported</font>

It has just been rebuilt for the first time in 3 years and has been quickly hacked to work with jQuery 1.11

And I have just discovered that code.google will no longer support binary downloads, so I cannot post the V1.5 zip file and you cannot download it. Feel free to pull down the full source and extract the pieces you need.

<font color='red'>Development/Downloads/Support have been transfered over to </font>[SourceForge](https://sourceforge.net/projects/dropdownchecklist/)**. Visit SourceForge for access to the latest updates. This code.google project remains solely for historical purposes.**<font color='red'>The google Issue list has been abandoned.</font>

### Usage ###
```
    $("#select_id").dropdownchecklist();
```
The existing select element with id 'select\_id' is replaced by a dropdown checkbox list widget.

See the **[DEMO](http://dropdown-check-list.googlecode.com/svn/trunk/doc/dropdownchecklist.html)** page for a detailed description, documentation, and live examples. This page is based on the functionality in the current, downloadable release.

See the **[TESTCASE](http://dropdown-check-list.googlecode.com/svn/trunk/doc/ddcl-tests.html)** page for a series of test cases that exercise DDCL in various ways. This page is based directly on the most current version checked into SVN, not on the stable release version.

### Limitations ###

1) Keyboard / Tab processing is iffy at best. I have found no reliable way of detecting loss of focus to another component in order to force an auto-close of the dropdown.

2) `<LABEL>` tags associated with the underlying `<SELECT>` just do not work, since the `<LABEL>` is wired to the original `<SELECT>`, not the DDCL component.  In particular, do not include the original `<SELECT>` within the span of the `<LABEL>` tag itself.

3) IFrame support is questionable

4) DDCL calculates size and position on widget initialization.  This only operates properly if the wrapper elements containing the `<SELECT>` are not hidden. Therefore, the use of DDCL within dynamic components that hide/show the wrapper element is problematic.

5) DDCL V1.4 was the last tested with IE6.  No future version of DDCL will test with IE6.

6) <font color='red'>DDCL V1.4 is <i>NOT</i> compatible with jQuery 1.8</font>

7) DDCL V1.5 has been tested with jQuery 1.11 - proper operation of any version of DDCL with jQuery 1.8, 1.9, and 1.10 is doubtful.

### History ###
See [change](http://dropdown-check-list.googlecode.com/svn/trunk/src/changes.txt) history.

Version 1.5 - requires jQuery/jQuery UI 1.11

Version 1.4 - requires jQuery 1.6.1, ui 1.8.13

Version 1.3 - copy of `<OPTION>` styling into the dynamic components

Version 1.2 (which never made it out of QA) - the various pop-up positioning problems reported in the issue log have been addressed

Version 1.1 - DDCL now based on jQuery 1.4.2, ui 1.8.4

Version 1.0 - the most significant difference between version 1.0 and 0.9 is the switch-over to jQuery ThemeRoller based styling. While many of the 0.9 class tags are still in place, some have been retired in favor of ThemeRoller settings. If you have customized your CSS based on 0.9, you will likely have to change some of your class name pattern matches.

### License ###
Licensed like jQuery, see http://docs.jquery.com/Licensing
