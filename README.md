我是光年实验室高级招聘经理。
我在github上访问了你的开源项目，你的代码超赞。你最近有没有在看工作机会，我们在招软件开发工程师，拉钩和BOSS等招聘网站也发布了相关岗位，有公司和职位的详细信息。
我们公司在杭州，业务主要做流量增长，是很多大型互联网公司的流量顾问。公司弹性工作制，福利齐全，发展潜力大，良好的办公环境和学习氛围。
公司官网是http://www.gnlab.com,公司地址是杭州市西湖区古墩路紫金广场B座，若你感兴趣，欢迎与我联系，
电话是0571-88839161，手机号：18668131388，微信号：echo 'bGhsaGxoMTEyNAo='|base64 -D ,静待佳音。如有打扰，还请见谅，祝生活愉快工作顺利。

<a href="http://getpat.io"><img src="https://raw.githubusercontent.com/la5nta/pat-website/gh-pages/img/logo.png" width="128" ></a>

[![Build Status](https://travis-ci.org/la5nta/pat.svg?branch=master)](https://travis-ci.org/la5nta/pat)
[![Windows Build Status](https://ci.appveyor.com/api/projects/status/tstq4suxfdmudl5l/branch/master?svg=true)](https://ci.appveyor.com/project/martinhpedersen/pat)
[![Go Report Card](https://goreportcard.com/badge/github.com/la5nta/pat)](https://goreportcard.com/report/github.com/la5nta/pat)

## Overview

Pat is a cross platform Winlink client with basic messaging capabilities.

It is the primary sandbox/prototype application for the [wl2k-go](https://github.com/la5nta/wl2k-go) project, and provides both a command line interface and a responsive (mobile-friendly) web interface.

It is mainly developed for Linux, but are also known to run on OS X, Windows and Android.

#### Features
* Message composer/reader (basic mailbox functionality).
* Auto-shrink image attachments.
* Post position reports with location from local GPS, browser location or manual entry.
* Rig control (using hamlib) for winmor PTT and QSY.
* CRON-like syntax for execution of scheduled commands (e.g. QSY or connect).
* Built in http-server with web interface (mobile friendly).
* Git style command line interface.
* Listen for P2P connections using multiple modes concurrently.
* AX.25, telnet, WINMOR and ARDOP support.
* Experimental gzip message compression (See "Gzip experiment" below).

##### Example
```
martinhpedersen@duo:~$ pat interactive
> listen winmor,telnet-p2p,ax25
2015/02/03 10:33:10 Listening for incoming traffic (winmor,telnet-p2p,ax25)...
> connect winmor:///LA3F
2015/02/03 10:34:28 Connecting to winmor:LA3F...
2015/02/03 10:34:33 Connected to WINMOR:LA3F
RMS Trimode 1.3.3.0 Follo.SE Oslo. Pactor & Winmor Hybrid Gateway
LA5NTA has 117 minutes remaining with LA3F
[WL2K-2.8.4.8-B2FWIHJM$]
Wien CMS via LA3F >
>FF
FC EM FOYNU8AKXX59 260 221 0
F> 68
1 proposal(s) received
Accepting FOYNU8AKXX59
Receiving [//WL2K test til linux] [offset 0]
>FF
FQ
Waiting for remote node to close the connection...
> _
```

### Gzip experiment

Gzip message compression has been added as an experimental B2F extension. The extension is implemented as a backwards compatible alternative to the ancient LZHUF compression.

This experiment is enabled by default and sessions between two Pat nodes (or other software supporting this B2F extension) will use gzip compression when transferring messages.

For more information, see <https://github.com/la5nta/wl2k-go#gzip-experiment>.

## Copyright/License

Copyright (c) 2014-2017 Martin Hebnes Pedersen LA5NTA

### Contributors (alphabetical)

* KD8DRX - Will Davidson
* LA3QMA - Kai Günter Brandt
* LA4TTA - Erlend Grimseid
* LA5NTA - Martin Hebnes Pedersen

## Thanks to

The JNOS developers for the properly maintained lzhuf implementation, as well as the original author Haruyasu Yoshizaki.

The paclink-unix team (Nicholas S. Castellano N2QZ and others) - reference implementation

Amateur Radio Safety Foundation, Inc. - The Winlink 2000 project

F6FBB Jean-Paul ROUBELAT - the FBB forwarding protocol

_Pat/wl2k-go is not affiliated with The Winlink Development Team nor the Winlink 2000 project [http://winlink.org]._
