# News website

A simple project aimed at learning and understanding microservices and the Spring Framework.

![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)

# Table of content
- [Database](#Database)
- [Back-end System](#Back-end-System)
- [User Interface](#User-Interface)
- [How to launch back-end using Docker](#How-to-launch-back-end-using-Docker)

## Database

The database is designed to be simplified as shown below:

![ERD](image/News-ERD.png)

With so few tables, database partitioning is unnecessary. However, for the purpose of studying microservice architecture, it has been divided as follows:

![ERD Split](image/News-ERD-split.png)

## Back-end System
Cách hoạt động back-end được mô tả trong hình sau
![ERD Split](image/BackendLogic.png)

## User Interface
Được viết bằng Angular. Phần này không được chi tiết lắm nhưng về cơ bản các chức năng vẫn hoạt động bình thường
### Home
![ERD Split](image/front-end-1.png)
### News details
![ERD Split](image/front-end-2.png)
### Management
![ERD Split](image/front-end-3.png)

## How to launch back-end using Docker

#### Docker compose v1
Update the environment variables in the service.env file then run.
````cmd
docker-compose --env-file service.env up -d
````
#### Docker compose v2
Replace environment variables directly in the docker-compose.yml file
````cmd
docker compose up -d
````
#### API Doccument [API Doccument](https://docs.google.com/document/d/1MILX7e_m3uf-qo26MZG9JSqRdvJ1B2_e/edit?usp=sharing&ouid=107957117387250494661&rtpof=true&sd=true)
