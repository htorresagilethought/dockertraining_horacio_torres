Create docker image
docker build -t myimage .

Create a Docker Container using the image. Assign "Site1" as container name and port "8085" to run the container.
docker run --name  Site1 -p  8085:80 myimage

Create a Docker Container using the image. Assign "Site2" as container name, port "8086" and "storename" as "Plano".
docker run --name  Site2 -p  8086:80 myimage -e "AppSettings:storename=Plano"