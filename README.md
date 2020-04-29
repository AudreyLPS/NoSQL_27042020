# NoSQL_27042020
Cours de la semaine 27-04-2020

### DOCKER

docker ps (-a)                          affiche toutes les instances de docker ( qui tournent ou non ) 

docker images (-a)                      afficher les images construites et intermédiaire

docker network ls                       liste des différents réseaux

docker-compose ps                       affiche tous les containers qui ont été lancés par docker-compose ( qui tournent ou non )


docker-compose up (-d)                  construire vos images si elles ne le sont pas déjà, et va démarrer vos dockers
                                        L’option -d, qui signifie "detach" fait tourner les conteneurs en tâche de fond
                                        
docker-compose build                    construire des images

docker-compose stop                     stop (mais ne supprime pas) vos conteneurs


docker build (-t <NAME>) <PATH>/<URL>   construire votre image, avec le nom et le PATH OU URL (cela peut être un repo git).
  
docker run (-d) (-p <hostPort>:<containerPort>) (--name <NAME>) <IMGNAME>/<IMGID> run crée le conteneur en utilisant l’image que vous indiquez
  
docker start <ID>/<NAME>                 uniquement des conteneurs qui sont déjà arrêtés, donc déjà build avec la commande run.
  
docker stop <ID>/<NAME>
  
docker exec -it <NAME>/<ID> <”/bin/bash”>      Cette commande vous permet de lancer un shell sur votre container