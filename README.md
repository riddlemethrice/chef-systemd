Systemd Chef Cookbook
=====================

[![Cookbook](http://img.shields.io/cookbook/v/systemd.svg)](https://github.com/nathwill/chef-systemd)
[![Build Status](https://travis-ci.org/nathwill/chef-systemd.svg?branch=master)](https://travis-ci.org/nathwill/chef-systemd)

A resource-driven [Chef][chef] cookbook for managing GNU/Linux systems via [systemd][docs].

<a name="toc">Table of Contents</a>
===================================

 - [Recommended Reading](#recommended-reading)
 - [Attributes](#attributes)
 - [Recipes](#recipes)
   - [Daemons](#daemon-recipes)
   - [Utilities](#utility-recipes)
 - [Resources](#resources)
   - [Daemons](#daemon-resources)
   - [Utilities](#utility-resources)
   - [Common Attributes](#common-resource-attributes)
     - [Exec](#common-exec)
     - [Kill](#common-kill)
     - [Resource Control](#common-resource-control)
     - [Unit](#common-unit)
     - [Install](#common-install)
     - [Drop-In](#common-drop-in)

<a name="recommended-reading">Recommended Reading</a>
=====================================================

 - This README
 - [Overview of systemd for RHEL 7][rhel]
 - [systemd docs][docs]
 - [Lennart's blog series][blog]
 - libraries in `libraries/*.rb`
 - test cookbook in `test/fixtures/cookbooks/setup`

<a name="attributes">Attributes</a>
===================================

too many to describe in detail ;).
in general, the attributes correspond to the related resource attributes.

<a name="recipes">Recipes</a>
=============================

 - **default**: no-op recipe

<a name="daemon-recipes">Daemon Recipes</a>
-------------------------------------------

 - **journald**: configure, manage systemd-journald
 - **journal\_gatewayd**: configure, manage systemd-journal-gatewayd
 - **logind**: configure, manage systemd-logind
 - **machined**: manage systemd-machined service
 - **networkd**: manage systemd-networkd service
 - **resolved**: configure, manage systemd-resolved
 - **timesyncd**: configure, manage systemd-timesyncd
 - **udevd**: configure, manage systemd-udevd

<a name="utility-recipes">Utility Recipes</a>
---------------------------------------------

 - **binfmt**: manage systemd-binfmt one-shot boot-up unit
 - **bootchart**: configure systemd-bootchart
 - **coredump**: configure systemd-coredump
 - **hostname**: configure, manage hostname with systemd-hostnamed
 - **locale**: configure, manage locale with systemd-localed
 - **real\_time\_clock**: configure system clock mode (UTC,local) with timedatectl
 - **sleep**: configure system sleep, suspend, hibernate behavior with systemd-sleep
 - **sysctl**: manage systemd-sysctl one-shot boot-up unit (apply sysctl at boot)
 - **system**: configure systemd manager system-mode defaults
 - **sysusers**: manage systemd-sysusers one-shot boot-up unit (set up system users at boot)
 - **timedated**: manage systemd-timedated one-shot boot-up unit (set time/date at boot)
 - **timezone**: configure, manage timezone with timedatectl
 - **user**: configure systemd manager user-mode defaults
 - **vconsole**: configure, manage virtual console font and keymap with systemd-vconsole

<a name="resources"></a>Resources
=================================

<a name="unit-resources"></a>Unit Resources
-------------------------------------------

<a name="systemd-automount"></a>**systemd\_automount**

<a name="systemd-device"></a>**systemd\_device**

<a name="systemd-mount"></a>**systemd\_mount**

<a name="systemd-path"></a>**systemd\_path**

<a name="systemd-service"></a>**systemd\_service**

<a name="systemd-slice"></a>**systemd\_slice**

<a name="systemd-socket"></a>**systemd\_socket**

<a name="systemd-swap"></a>**systemd\_swap**

<a name="systemd-target"></a>**systemd\_target**

<a name="systemd-timer"></a>**systemd\_timer**


<a name="daemon-resources"></a>Daemon Resources
-----------------------------------------------

<a name="systemd-journald"></a>**systemd\_journald**

<a name="systemd-logind"></a>**systemd\_logind**

<a name="systemd-resolved"></a>**systemd\_resolved**

<a name="systemd-timesyncd"></a>**systemd\_timesyncd**



<a name="utility-resources"></a>Utility Resources
-------------------------------------------------

<a name="systemd-bootchart"></a>**systemd\_bootchart**

<a name="systemd-coredump"></a>**systemd\_coredump**

<a name="systemd-sleep"></a>**systemd\_sleep**

<a name="systemd-system"></a>**systemd\_system**

<a name="systemd-user"></a>**systemd\_user**


<a name="misc-resources"></a>Miscellaneous Resources
----------------------------------------------------

<a name="systemd-binfmt-d"></a>**systemd\_binfmt\_d**

<a name="systemd-modules"></a>**systemd\_modules**

<a name="systemd-networkd-link"></a>**systemd\_networkd\_link**

<a name="systemd-sysctl"></a>**systemd\_sysctl**

<a name="systemd-sysuser"></a>**systemd\_sysuser**

<a name="systemd-tmpfile"></a>**systemd\_tmpfile**

<a name="systemd-udev-rules"></a>**systemd\_udev\_rules**


<a name="common-resource-attributes"></a>Common Resource Attributes
-------------------------------------------------------------------

<a name="common-exec"></a>**Exec**

<a name="common-kill"></a>**Kill**

<a name="common-resource-control"></a>**Resource Control**

<a name="common-unit"></a>**Unit**

<a name="common-install"></a>**Install**

<a name="common-drop-in"></a>**Drop-In**


--
[blog]: http://0pointer.de/blog/projects/systemd-for-admins-1.html
[chef]: https://chef.io
[docs]: http://www.freedesktop.org/wiki/Software/systemd/
[rhel]: https://access.redhat.com/articles/754933
