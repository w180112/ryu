## Link backup and broadcast storm prevention

The link backup application is an implementation can detect any link disconnection and find a new path between two hosts. 

The broadcast storm prevention application can detect any broadcast storm in topology and block it.

If you want to excute broadcast storm prevention application, just type
	ryu-manager --observe-links <ryu path>/ryu/ryu/app/w180112/broadcast_storm_preventtion/broadcast_storm.py

If you want to excute link backup application, just type
	ryu-manager --observe-links <ryu path>/ryu/ryu/app/w180112/link_backup/link_monitor.py

### Note

1. All applications are based on networkx, so pip install networkx==1.11 before use.
2. Due to some link caculating mechanism, execute mininet before running ryu