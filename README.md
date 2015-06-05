# Mumudvb_monitor

#Munin

Install <p>
cp munin/mumudvb /usr/share/munin/pugins/
ln -s /usr/share/munin/pugins/mumudvb /etc/munin/plugins/mumudvb_8000  # for a card0
ln -s /usr/share/munin/pugins/mumudvb /etc/munin/plugins/mumudvb_8001  # for a card1
.....

Relevant mumudvb.cfg:
  unicast=1         # Activate the internal webserver
  port_http=8000+%card
  
