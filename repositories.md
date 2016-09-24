---
layout: default
title: 11. Software Repositories - Adding and Managing Package Repositories
permalink: /repositories/
---

# 11. Software Repositories

As mentioned in the previous chapter, the package manager installs software by fetching packages from software repositories, therefore the software available for easy installation via the package manager depends on the configured repositories.

A software repository is a collection of RPM packages (the openSUSE packaging format) and metadata for the available packages. Usually repositories are on online servers, but it can also be on a CD/DVD or on other media.

## 11.1 Managing Repositories

Respositories can be added, removed and configured via YaST, in the module called Software Repositories.

<center><a href="{{ site.baseurl | append: '/images/screenshots/yast-repos.png' | replace: '//', '/' }}" rel="thumbnail"><img src="{{ site.baseurl | append: '/images/screenshots/yast-reposb.png' | replace: '//', '/' }}" alt="repos" class="pic" /></a></center>

### 11.1.1 Adding Repositories

The official repositories are pre-configured, but many unofficial repositories exist and can be added too.

<div class="obs">
<table>
<tbody>
<tr>
<td><img src="{{ site.baseurl | append: '/images/pics/obs.png' | replace: '//', '/' }}" alt="obs" /></td>
<td>Add repositories with care.
<ul>
<li>Unofficial repositories might include experimental packages</li>
<li>Not all repositories are mutually compatible</li>
<li>The risk level of a repository can change over time</li>
<li>Too many repositories makes the package manager slower</li>
</ul>
</td>
</tr>
</tbody>
</table>
</div>

The easiest and safest way to add repositories is using the list of online community repositories in YaST. This provides you with a selection of popular and quite safe repositories to choose from:

<div class="sti">YaST => Software => Software Repositories => Click on "Add" => Select "Community Repositories" and click "Next"</div>

<center><video src="video/repos114.ogv" controls>  

<center><a href="{{ site.baseurl | append: '/images/screenshots/community-repos.png' | replace: '//', '/' }}" rel="thumbnail"><img src="{{ site.baseurl | append: '/images/screenshots/community-reposb.png' | replace: '//', '/' }}" alt="repos" class="pic" /></a></center>

<b>Your web browser does not support the HTML5 video element and/or Ogg Theora format.

Try Firefox, Konqueror or Opera.</b>

<a href="video/repos-full.ogv">Download video for local viewing (4.3 MB)</a>
</video></center>  

Note that the <i>openSUSE BuildService</i> is a service for the community to build and share packages. <i>openSUSE BuildService repositories are unofficial and unsupported</i>. Use at your own risk.

### 11.1.2 Recommended Repositories

You should always have the four <i>official</i> repositories (which are configured out of the box).<br/>

<ul>
	<li><b>Main Repository (OSS)</b></li>
	<li><b>Main Repository (NON-OSS)</b></li>
	<li><b>Main Update Repository</b></li>
	<li><b>Main Update Repository (NON-OSS)</b></li>
</ul>

Additionally I recommend adding the following <i>unofficial</i> repositories from the Community Repositories list, for having a good balance of software supply and stability for most users.

<ul>
	<li><b>Packman Repository</b></li>
	<!--<li><b>openSUSE BuildService - KDE:Extra</b></li>-->
</ul>

<div class="tip">
<table>
<tbody>
<tr>
<td><img src="{{ site.baseurl | append: '/images/pics/tip.png' | replace: '//', '/' }}" alt="tip" /></td>
<td>Still missing a package?<br /><br />

You can search for packages/repositories on the openSUSE BuildService here:<br />

<a href="http://software.opensuse.org/search" target="_blank">http://software.opensuse.org/search</a><br /><br />

This package search engine also includes the Packman repository:<br />

<a href="http://webpinstant.com" target="_blank">http://webpinstant.com</a><br /><br />

Remember to add unofficial repositories with care!</td>
</tr>
</tbody>
</table>
</div>

### 11.1.3 Vendor Change Updates

Updating installed packages from one repository to versions from a different repository with a different <i>vendor</i>, is a little bit complicated. Read about it here:

<a href="http://en.opensuse.org/SDB:Vendor_change_update" target="_blank">http://en.opensuse.org/SDB:Vendor_change_update</a>

## 11.2 Repository Management in the Terminal

If you wish, you can manage your repositories via a terminal too.

Add a repository with auto-refresh enabled <i>zypper addrepo -f [URL] [Alias]</i>. Example:

<div class="clroot">zypper addrepo -f http://packman.inode.at/suse/openSUSE_Leap_42.1/ packman</div>

Disable a repository <i>zypper modifyrepo -d [URL|Alias]</i>. Example:

<div class="clroot">zypper modifyrepo -d Packman</div>

Remove a repository <i>zypper removerepo [URL|Alias]</i>. Example:

<div class="clroot">zypper removerepo http://packman.inode.at/suse/openSUSE_Leap_42.1/</div>

List configured repositories, showing  details (priorities, URL, etc.):

<div class="cl">zypper repos -d</div>

See <i>man zypper</i> for more.

<div class="cl">man zypper</div>

Or for help on indvidual commands use for example:

<div class="cl">zypper addrepo --help</div>