# aspIRCd Changes

## Changes since Version 4.0.5

- [] - Add fake /list



- [X] - Move m_locops module to extensions.
- [X] - Added usermode +O which will hide oper from /whois for non oper accounts
- [X] - Added module chm_insecure, which requires users to use SSL to join channels unless mode +U is set
- [X] - Move show_whois into core
- [X] - Remove unused modules/extensions
- [X] - Added --with-shared-sqlite option for low end vps and Raspberry Pi style boards (requires package libsqlite3-dev)
- [X] - Added datarootdir that was missing
- [X] - Allow exact PID file prefix to be specified
- [X] - Removed smallnet option as never used



## Changes since Version 4.0.1

- [X] - Added usermode +I which will hide idle from /whois output for non oper accounts
- [X] - Reinstated configuration option for the nick of the SASL agent
- [X] - Moved ip_cloaking to modules and renamed to m_cloak. Automatically loaded now
- [X] - Dix gnutls error with version 3+
- [X] - Update openSSL 
- [X] - Removed unused cloaking
- [X] - Show users the RESV reason
- [X] - Purged local channels (not really used)
- [X] - Hard coded chm_sslonly into the core
- [X] - Fixed extb_channel bug where if banned target channel has +s or +p set it wouldn't work
- [X] - Use NAMELEN instead of NICKLEN when accessing Client->name because it could in theory be a HOSTLEN length string.

## Changes since Version 4.0.0-1
 
- [X] - Add vhost for opers support, requiring opers to identify with nickserv firstly
- [X] - Remove zip linking support
- [X] - Fix Compile errors
- [X] - Removed oponlymsg and named staffonly (mode +m prevents none IRCops messaging you)
- [X] - Use sha-512 for SSL
- [X] - Remove DES support for mkpasswd
- [X] - Upgrade sqlite to 3.8.10
- [X] - Remove last update to m_sasl.c
- [X] - Added another cloaking module

## Changes since Version 3.5.9

- [X] Change who can set selected channel modes
- [X] Remove NOKICKOPER(Channel mode +M) from core and make a module
- [X] Allow self-devoicing (enbaled/disabled via config)
- [X] Moved selected extensions to modules   
- [X] Fix halfop permissions (Allow self-dehalfop)
- [X] Show a client's unique ID on connect & whois
- [X] Add static parts
- [X] Remove m_roleplay
- [X] Add sasl_usercloak
- [X] Added m_forcequit (Allows admins to /forcequit users remote/locally and IRCOP's locally only)
- [X] Added show_whois - usermode +W which will notify you when someone does a /whois on you
- [X] Added a idle time feature for IRCOPs, if Idle for longer than set time they'll be removed from /stats p (defaults: 2hours)
- [X] Added extb_hostmask - Hostmask extban type: bans all users matching a given hostmask
- [X] Reverted ip_cloaking module back to original state
