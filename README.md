---------------------------------------------------
Description of the File and Folders present on Dory
---------------------------------------------------


Cloudlus server for Fuelcycle.org and Cyclist
============================================

- something like: `./cloudlus -addr=http://cycrun.fuelcycle.org serve &> serve.log &` -> relaunch http://cycrun.fuelcycle.org if not working try with cycrun.fuelcycle.org:80 
- `launch.sh N` -> launch N worker for fuelcycle.org cloudlus
- `worker-x` -> folder where fuelcycle worker works
- `cyc-cde.tar.gz` worker base software
- removing all Month calculation : `ls -al |grep XxX |grep zip |cut -d":" -f2 |cut -d" " -f2 |xargs rm`

Meghan Cloudlus Server
======================

- `git/mbmore` -> meghan cloudlus
- start cloudlus: `./cloudlus -addr 0.0.0.0:1441 serve &> server.log &`
- launch worker: docker run mbmcgarry/mbmore &> workerN.log &


Baptiste Cloudlus Server: `BaM` folder
======================================

- `optim1` -> cloudlus server for optimisation
- HTC_tool: compilation of cloudlus stuff



Storage of the Cyclus/Cycamore installation deb-package
=======================================================

- `cyclus-deb_* + fileserv` -> debian package cloud storage
- start the http storage server : nohup ./cyclus-deb_launch_http_server.sh &> http.server.log &


