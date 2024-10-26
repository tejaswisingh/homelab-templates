> ⚠️ Before you deploy 

You would need to create five docker volumes that the compose utilizes.

Run the following commands on your host:-
```bash
docker volume create authentik_database
docker volume create authentik_redis
docker volume create authentik_media
docker volume create authentik_certs
docker volume create authentik_custom_templates
```

Also, this docker-compose assumes your have a reverse proxy setup already like [NginxProxyManager](https://github.com/tejaswisingh/homelab-templates/tree/main/docker-compose/nginxproxymanager) hence the port exposed containers are networked to the reverse proxy.