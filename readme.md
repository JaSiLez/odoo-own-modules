# Mini doc.:

## Requirements:
* Docker & Docker Compose
* Dockerized Odoo

### Start the server:
```shell
git clone -b 14.0 git@github.com:iterativo-git/dockerdoo.git && cd dockerdoo
docker-compose -f docker-compose.yml -f dev-standalone.yml up
```


### To create a new module:
  Identicate the container:
  ```shell
  sudo docker ps
  ```
  Selecting it by container ID:
  ```shell
  sudo docker exec -it <container_id> bash
  ```
  Creating a new module with Odoo:
  ```shell
  odoo scaffold <new_name_module> mnt/extra-addons/etc...
  ```






