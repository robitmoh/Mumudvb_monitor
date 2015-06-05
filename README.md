# Mumudvb_monitor

#Munin

Install <p>
cp munin/mumudvb /usr/share/munin/pugins/<p>
ln -s /usr/share/munin/pugins/mumudvb /etc/munin/plugins/mumudvb_8000  # for a card0<p>
ln -s /usr/share/munin/pugins/mumudvb /etc/munin/plugins/mumudvb_8001  # for a card1<p>
.....<p>

Relevant mumudvb.cfg:<p>
  unicast=1         # Activate the internal webserver<p>
  port_http=8000+%card<p>
  
