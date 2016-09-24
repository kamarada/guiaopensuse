---
layout: default
title: 14. Browser Plugins - Install Plugins For Your Web Browser Such As Flash and Java
permalink: /browserplugins/
---

# 14. Browser Plugins

Many websites require various browser plugins to be installed to function as expected. Here are some plugins that you may want to install.

<div class="tip">
<table>
<tbody>
<tr>
<td><img src="{{ site.baseurl | append: '/images/pics/tip.png' | replace: '//', '/' }}" alt="tip" /></td>
<td>If the concepts of <i>package manager</i> and <i>repositories</i> are foreign to you, revisit the chapters <a href="installpackage.php">Installing Software</a> and <a href="repositories.php">Software Repositories</a>.</td>
</tr>
</tbody>
</table>
</div>

## 14.1 Adobe Flash

Install the package <b>flash-plugin</b>, if you need Flash support for some online videos, games and other things (<i>Adobe Flash Plugin Repository</i> is required).

Installing Flash in the terminal:

<div class="clroot">zypper addrepo -f http://linuxdownload.adobe.com/linux/x86_64/ adobe-flash-plugin</div>

<div class="clroot">zypper install flash-plugin</div>

You will get a warning about a missing GPG-key.

## 14.2 Java

Java web applets are used for games, home banking in some countries, and various other things.

Install the package <b>java-1_8_0-openjdk-plugin</b> with the package manager if it isn't already installed.

Installing Java browser plugin in the terminal:

<div class="clroot">zypper install java-1_8_0-openjdk-plugin</div>

## 14.3 Video and Audio Streaming

To get support for various multimedia streams in Firefox and other browsers, install the package <b>xine-browser-plugin</b> (<i>Packman Repository</i> required).

Installing multimedia plugin in the terminal:

<div class="clroot">zypper install xine-browser-plugin</div>

## 14.4 Microsoft Silverlight

Microsoft have created something called Silverlight to compete with Adobe Flash in making the web require proprietary extensions.

As you'd expect Microsoft do <i>not</i> provide an official plugin for GNU/Linux, but there is something called <a href="http://fds-team.de/cms/articles/2013-08/pipelight-using-silverlight-in-linux-browsers.html" target="_blank">Pipelight</a> bringing Microsoft Silverlight to the GNU/Linux platform. You can find Pipelight packages for openSUSE <a href="http://software.opensuse.org/package/pipelight" target="_blank">here</a>

Netflix will play in the latest Google Chrome Browser, without any need for Microsoft Silverlight.

## 14.5 Google Voice and Video Chat

Google provide voice and video chat with Google services on GNU/Linux with a browser plugin. Download the RPM files for openSUSE here:

<a href="http://www.google.com/chat/video">http://www.google.com/chat/video</a>