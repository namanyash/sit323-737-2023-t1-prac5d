# sit323-737-2023-t1-prac5d

## Starting application

TO install node modules run the following command
`npm install`

Run the following command to build and run the project using docker-compose
`docker-compose up -d`

To test connection use the to the following URL
`http://localhost:8080/getToken`

## To test the health check

sh into the `web1` container using the following command
`docker exec -it sit323-737-2023-t1-prac5d-web1-1 sh`

Update the container
`apt-get update`

Install `inetutils-ping` in the container
`apt-get install inetutils-ping`
_You may need to press the key 'y' during the installation process_

Ping the web2 container from web1
`ping sit323-737-2023-t1-prac5d-web2-1`
