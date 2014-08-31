irssi proxy backlog sending
============

Original source from  http://wouter.coekaerts.be/site/irssi/proxy_backlog

Uses server-time tagging http://ircv3.atheme.org/extensions/server-time-3.2

settings and defaults are:

```proxy_backlog_lines 10``` Number of lines to send (does send only 10 last lines, change to e.g. 100 ?)

```proxy_backlog_debug OFF``` Set ON for more verbose processing of channels CAUTION! Use this only when really need to debug issues.

To request new backlogs, send (case sensitive) ```/CTCP -proxy- IRSSIPROXY BACKLOG SEND```

If there was something to send, ```-!- BACKLOG SENDING DONE``` tag is added to irssi window to find location what has been already sent.

Change of day needs still some improvements to work properly.

Tested with follogin clients:

  - works: communi-sailfish 0.8 > https://github.com/communi/communi-sailfish/releases/tag/v0.8
  - doesn't work: ChatZilla (Firefox addon)

