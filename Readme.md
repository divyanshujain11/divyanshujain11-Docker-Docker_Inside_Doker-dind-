Step 1:
Installing Docker Image docker:dind

        yum install docker:dind

 ![image](https://github.com/divyanshujain11/divyanshujain11-Docker-Docker_Inside_Doker-dind-/assets/77712311/9c121d14-5656-49c8-9297-2620ebcf6f7d)


Step2:
Launching a container with privileged (--privileged) power by docker:dind image in deteched mode (-d)

        docker run --privileged -d --name dind-container docker:dind


![image](https://github.com/divyanshujain11/divyanshujain11-Docker-Docker_Inside_Doker-dind-/assets/77712311/9f69266d-9bfe-4c24-8d7c-fba47ddf75aa)



step 3:
Execute docker container (dind-container) with shel command in the container
        
        docker exec -it dind-container sh


![image](https://github.com/divyanshujain11/divyanshujain11-Docker-Docker_Inside_Doker-dind-/assets/77712311/d320dab9-ebe8-4793-8b1c-f23d595698f7)



step 4:
Launch new Container in the docker container(dind-container)

        docker pull centos:7
        docker run -it --name dockerInTheDocker centos:7


![image](https://github.com/divyanshujain11/divyanshujain11-Docker-Docker_Inside_Doker-dind-/assets/77712311/bfe2a87f-8bcc-4cc1-a602-25d26944b655)





