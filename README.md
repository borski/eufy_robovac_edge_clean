# eufy robovac edge cleaning

Implementation of edge cleaning in home assistant from the eufy robovac, using both the eufy robovac repo (cloned) and the vacuum repo (cloned) I then modified these files to include the functions for edge cleaning. You should only have to deposit these folders/file structure into your custom_components folder, preform a full reboot, and the functionality should appear under the services menu.

## Getting Started:

In this guide I will be implementing edge cleaning on the eufy robovac

### Prerequisites:

* Home Assistant with HACS installed
* A robovac that is currently using the eufy_robovac integration in hacs
* Local access to your custom_components folder
* The ability to reboot your server

```
Known working Models:
Eufy Robovac 35c
```

### Implementation:

Follow Guide on installing HACS into home assistant if you have not already done so.

Enable the samba share addon or otherwise gain access locally to your "custom_component" folder.

Copy and paste the folder (not the files at the top level, just the 2 folders (eufy_robovac, vacuum) into your custom components folder.

Fully reboot your home assistant server.

Test functionality in the services menu for your robovac.

## Running the tests

Developer tool > services > 
robovac.edge_clean
entity_id: vacuum.your_vacuum

### Break down into end to end tests

I copy/pasted from the home assistant source code the vacuum integration.
I then added the additional services, and backend for the edge cleaning as seen in the git-hub example seen below
I then modified the Eufy_robovac integration to include, and enable the edge cleaning functionality.
Then, lastly, I modified the robovac lovelace card to include this functionality, as that card already had SPOT cleaning functionality, and just changing that function to do EDGE cleaning instead, it works as expected.

```
[changes made from vacuum integration](https://github.com/home-assistant/core/pull/25483/files#diff-6903b845a32a9975ae29b8f6389a34da)
```

## Built With

* Python
* Notepad++


## Authors

* **The Home Assistant Team** - *All the Vacuum integration work* - (https://community.home-assistant.io/)
* **mitchellrj** - *All the eufy_robovac integration work* - (https://github.com/mitchellrj/eufy_robovac)
* **JXGA** - *For leaving me the tiniest bit of crumbs to do all this* - (https://github.com/home-assistant/core/pull/25483/files#diff-6903b845a32a9975ae29b8f6389a34da)


## License

I can has License Please? No seriously, what do I do here? anything? I'm just following the good old template

## Acknowledgments

* The Home Assistant Team
* mitchellrj
* JXGA
* Mom
* My Loving Wife

