# Linux-Forensics-Tools-Capabilities
This repository contains simple CSV file which list the artifacts gather by Linux forensic tools

I ran below open source IR tools on red hat to check various artifacts it collects from endpoint.
UAC -> Unix-like Artifacts Collector
catScale  ->
varc -> Volatile Artifact Collector 
cylr -> Live Response Collection 

As far as capabilites are concern I have put it in csv file kept here, feel free to add yout observation.

Also screenshot here just to get idea of logs

UAC -> https://github.com/tclahr/uac
Collects lot of data live data like processes, network connection, list of executable and hashes,  installed packages, container , VM , config files from /etc directory
bodyfile is important for creating timeline of activities.

catScale -> https://github.com/WithSecureLabs/LinuxCatScale
Similart to UAC it collect volite data, alos captures hidden file, persistence entries and also log files from /var/log/ directory
important feature of CatScale is, it lets u setup ELK instace so you can help you for analysis

varc -> https://github.com/cado-security/varc
Good tool for collecting live data like processes network. Also collects various directories like /etc/ /var/ 
along with this it takes memory dump of all processes

CyLR -> https://github.com/orlikoski/CyLR?tab=readme-ov-file
CyLR collects lot of files from various directories includes config files from /etc/, logs from /var/log/
It also collects USNjournal $UsnJrnl.
