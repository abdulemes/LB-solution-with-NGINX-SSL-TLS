# Project Workflow

## Configuring NGINX as a load balancer

Step 1 - An ubuntu EC2. instance was spinned for NGINX load balancer. 

Step 2 - The /etc/hosts file was updated with web servers names and thier IP address.

![IMG_9885](https://user-images.githubusercontent.com/93732510/164973227-c6d82704-7892-4628-98fd-5118cdb3863d.jpg)

Step 3 - NGINX was installed.

![IMG_9863](https://user-images.githubusercontent.com/93732510/164973097-7dc193bd-688c-4be2-946e-d9b75af377b8.jpg)

Step 4 - The NGINX configuration file was updated with the web servers names defined in /etc/hosts file.

![IMG_9884](https://user-images.githubusercontent.com/93732510/164973506-3b919d47-c4be-4c8c-ad51-6124aadc96fb.jpg)

Step 4 - NGINX was restarted for the changes to take effect. 

![IMG_9886](https://user-images.githubusercontent.com/93732510/164973596-de41dac4-0d8f-419b-982f-ba57e3b63ab4.jpg)

## Configuring secured connection using ssl/tls certificates with a domain name

Step 1 - Elastic IP address was created and associated with NGINX LB.

![IMG_9873](https://user-images.githubusercontent.com/93732510/164973788-83b48600-da6b-4c9d-b6e6-8b63f7a5b944.jpg)

Step 2 - A record was updated to point to NGINX LB using elastic IP.

![IMG_9874](https://user-images.githubusercontent.com/93732510/164973825-5280211d-dc2a-4a42-b414-3e627abbfd3d.jpg)

Step 3 - The web servers were viewed from browser using the domain name using http.

![IMG_9887](https://user-images.githubusercontent.com/93732510/164973976-3c58c561-ad5c-4e1f-9981-245f520d081f.jpg)

Step 4 - NGINX configuration file was updated with the web servers domain name.

Step 5 - Snapd was check verifying it is running and active.

![IMG_9888](https://user-images.githubusercontent.com/93732510/164974129-0746233c-884b-41ab-ad63-5557a89b770e.jpg)

Step 6 - Cerbot was installed and certificate requested.

![IMG_9890](https://user-images.githubusercontent.com/93732510/164974221-0bbd9355-9bf0-42f5-8a69-2bc5b16b8e6f.jpg)

![IMG_9891](https://user-images.githubusercontent.com/93732510/164974240-1f11da5c-bdb1-475d-88f1-e52feb5bdd8f.jpg)

Step 7 - The webserver was checked using https in the browser and certificate verified.

![IMG_9892](https://user-images.githubusercontent.com/93732510/164974308-19767a8b-be5b-412e-bbd1-befe2dd68b11.jpg)

![IMG_9893](https://user-images.githubusercontent.com/93732510/164974367-91012f1e-4cde-4079-a309-1ede652bd581.jpg)

Bonus Step - Periodical renewal of ssl/tsl certificates was setup.

![IMG_9895](https://user-images.githubusercontent.com/93732510/164974456-e91b6cb9-2210-4ae6-8124-bf134b699542.jpg)
