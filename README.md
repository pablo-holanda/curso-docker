# curso-docker

# Estrutura de redes

* Web Network
 
    Utilizada para a comunicação entre os aplicativos web.
    
    Comando: `docker network create -d bridge web_network` 
    
* DB App Laravel Network
 
    Rede isolada para o banco da aplicação Laravel.
    
    Comando: `docker network create -d bridge db_app_laravel`
    
# Volumes

* Web Apps Volume

    Comando: `docker volume create web_apps` 
    
* DB Laravel Volume

    Comando: `docker volume create db_laravel` 
    
* Laravel data Volume

    Comando: `docker volume create laravel_data` 