#distributed-consensus

==================Run the code=============================
Terminal A:
cd ~/Desktop/ee597/core/
sudo service core-daemon start
sudo core-gui --start ~/Desktop/ee597/uavs-targets/uav8-notrack.imn

Terminal B:
cd ~/Desktop/ee597/uavs-targets/
bash start_tracking.sh none
bash start_tracking.sh udp
bash start_testing.sh

=================Stop the code=============================
Terminal A:
sudo service core-daemon stop

Terminal C:
cd /tmp/
sudo rm *.txt *.log