---
layout: default
title: "Appendix B: Games - Playing Games on openSUSE"
permalink: /games/
---

# Appendix B: Games

Not all major, mainstream games run natively on GNU/Linux, but there are still plenty of gaming options.

<center><img src="{{ site.baseurl | append: '/images/pics/spil.jpg' | replace: '//', '/' }}" alt="spil" class="pic" /></center>

## B.1 Native GNU/Linux Games

### B.1.1 openSUSE Build Service Games Repository

Some games are included in the official openSUSE repositories, but the Games repository on the openSUSE Build Service includes a lot more games. You can easily add this repository via the list of Community Repositories as described in the chapter about <a href="repositories.php">Software Repositories</a>

Or add the games repository using the command line:

<div class="clroot">zypper addrepo -f http://download.opensuse.org/repositories/games/openSUSE_Leap_42.1/ games</div>

### B.1.2 Steam Gaming Platform and Store

The <a href="http://store.steampowered.com/browse/linux/" target="_blank">Steam gaming platform and store</a> is available for GNU/Linux.You can find packages of it <a href="http://software.opensuse.org/package/steam" target="_blank">here</a>

### B.1.3 Desura

The Desura distribution service for gamers provides easy access to non-free indie games, see:

<a href="http://www.desura.com" target="_blank">http://www.desura.com</a>

### B.1.4 Other GNU/Linux Gaming Resources

Linux Game Publishing buy titles and port them to GNU/Linux, see:

<a href="http://www.linuxgamepublishing.com" target="_blank">http://www.linuxgamepublishing.com</a>

Lots and lots more of free and non-free games exist - some small and simple, others quite big, and many very good. Check out some of these sites:

<a href="http://happypenguin.org/" target="_blank">http://happypenguin.org/</a>

<a href="http://www.tuxgames.com/" target="_blank">http://www.tuxgames.com/</a>

<a href="http://www.penguspy.com/" target="_blank">http://www.penguspy.com/</a>

<a href="http://www.lgdb.org/" target="_blank">http://www.lgdb.org/</a>

<a href="http://www.linuxgamingworld.com/" target="_blank">http://www.linuxgamingworld.com/</a>

## B.2 Running MS Windows Games

Some software available for GNU/Linux allows you to run games developed for MS Windows on GNU/Linux - ease of use and success rate may vary - however, the more popular the game, the more likely it is to be supported.

### B.2.1 Wine

Wine (Wine Is Not an Emulator) is the first option, it's free software installable via the package manager. See the Wine app database for information on running individual games:

<a href="http://appdb.winehq.org/appbrowse.php?iCatId=2" target="_blank">http://appdb.winehq.org/appbrowse.php?iCatId=2</a>

Wine is a command line application, the syntax is:

<div class="cl">wine /path/to/setup.exe</div>

### B.2.2 PlayOnLinux

<a href="http://www.playonlinux.com/" target="_blank">PlayOnLinux</a> is based on Wine and lets you easily install and use (some) MS Windows Games. You can find packages of PlayOnLinux in the above mentioned Games repository.

### B.2.3 CrossOver Games

A second option is CrossOver Games which is an effort based on Wine. See:

<a href="http://www.codeweavers.com/products/cxgames/" target="_blank">http://www.codeweavers.com/products/cxgames/</a>

<!--
### B.2.4 Cedega

Another option that lets you run MS Windows games is Cedega. They have some MS Windows games officially certified for being ran this way. See:

<a href="http://www.cedega.com" target="_blank">http://www.cedega.com/</a>
-->

## B.3 Emulators

Numerous emulators exist, making it possible to run many old classic games of other platforms on GNU/Linux. For example:

<ul>
  <li>Amiga (UAE)</li>
  <li>Arcade (MAME)</li>
  <li>Atari (Stella, Steem)</li>
  <li>Commodore 64/128 (VICE)</li>
  <li>MS DOS (DOSBox, DOSEMU)</li>
  <li>Nintendo (infones, bsnes, nestopia)</li>
  <li>Play Station (pcsx, pcsx2)</li>
  
</ul>

<div class="tip">
<table>
<tbody>
<tr>
<td><img src="{{ site.baseurl | append: '/images/pics/tip.png' | replace: '//', '/' }}" alt="tip" /></td>
<td>Usually you can only do this legally, if you own the original hardware/have a licence for it.</td>
</tr>
</tbody>
</table>
</div>