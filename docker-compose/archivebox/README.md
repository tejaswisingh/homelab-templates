> ⚠️ Before you deploy 

The only step that needs to be performed before launching this container is to create two docker volumes that the compose utilizes.

Run the following commands on your host:-
```bash
docker volume create archivebox_data
docker volume create archivebox_sonic_data
```
