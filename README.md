# eufy_robovac_edge_clean
 Implementation of edge cleaning in home assistant from the eufy robovac, using both the eufy robovac repo (cloned) and the vacuum repo (cloned) I then modified these files to include the functions for edge cleaning. You should only have to deposit these folders/file structure into your custom_components folder, preform a full reboot, and the functionality should appear under the services menu.


Implementation:

Follow Guide on installing HACS into home assistant if you have no already done so.

Enable the samba share addon or otherwise gain access locally to your "custom_component" folder.

Copy and paste the folder (not the files at the top level, just the 2 folders (eufy_robovac, vacuum) into your custom components folder.

Fully reboot your home assistant server.

Test functionality in the services menu for your robovac.
