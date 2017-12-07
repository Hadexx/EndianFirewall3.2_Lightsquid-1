# Endian Firewall 3.2.x





Lightsquid Report
=============
Addon for Endian Firewall 3.2, install report Lighsquid for Squid logs.


Version:
--------
v.2.0 ( for Endian versions 3.2.1, 3.2.2 and 3.2.4).


Requirements/optinal:
--------
- Requires: Acess your firewall trought SSH Connection.


Installation:
--------

Downloading:

    curl -Lo lightsquid-endian3-2.0-1.x86_64.rpm LINK
    
Installation:

    rpm -Uvh lightsquid-endian3-2.0-1.x86_64.rpm

Create user lighsquid password:

- Run script in ssh: /usr/local/bin/lightsquid-password.sh or lightsquid-password.sh. 
- type your password to acess the reports and press ENTER.

Direct Acess to reports:

Link: https://YOUENDIANGREENIP:10443/lightsquid   (Ex: https://192.168.0.15:10443/lightsquid )

Unnistall:
--------

    rpm -e lightsquid-endian3
    
Other information:
------------------

- This installation run together with sarg, no need uninstall sarg report.
- To Active this report, You need select check box "Ativar Lightsquid" and click "Save" on Endian Firewall control Painel, on menu Logs and reports -> Proxy -> HTTP report.
- Reports will be generated every day automatically.
  
  
