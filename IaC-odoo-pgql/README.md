# 📄Repo theme
In this lab , i try to deploy the Odoo ERP and its PostgreSQL database
using the documentation on https://hub.docker.com/_/odoo .

I write a docker-compose.yml file https://github.com/ImaneKABKAB/formation-eazytraining-devops-docker/blob/main/IaC-odoo-pgql/docker-compose.yml where i list :

 - A web service representing the Odoo ERP  .
 
 - A db service representing the postgresql database with its environment variables like POSTGRES_DB and POSTGRES_PASSWORD .
 
 - Volumes of type bind mount and volumes so that data and configuration informations become persistent .  
 
 - A network named odoo_network of type bridge to insure communication between the 2 services
 
 Here is the website image 
 ![private](https://github.com/ImaneKABKAB/formation-eazytraining-devops-docker/blob/main/images/Iac1.png)
 ![private](https://github.com/ImaneKABKAB/formation-eazytraining-devops-docker/blob/main/images/Iac2.png)
