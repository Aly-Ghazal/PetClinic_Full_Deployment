# PetClinic Full Deployment

## Description

The web app, "Pet Clinic," is a comprehensive system designed to manage veterinary clinics and their daily operations. It allows veterinarians, staff, and pet owners to efficiently interact, schedule appointments, manage pet records, and facilitate seamless communication.

## user manual

1- run the first Playbook "PlaybookCreateUser.yml"

    `ansible-playbook PlaybookCreateUser.yml`

   to create pet-clinic user and download java jdk-18

2- run the second playbook "PlaybookInstallRequiredTools.yml"

    `ansible-playbook PlaybookInstallRequiredTools.yml -K`

   and this time you need to enter pet-clinic user's password which "1234"

   to install tomcat and make it listen to port 9090 then restart it and install jenkins too, make it listen 3000 and start it up

3- open your browser and insert this url `http://localhost:3000/`

and

- setup Jenkins

- create a new pipeline Job

- then copy jenkinsfile to pipeline script

- then build it

4- open new tab and insert this url `http://localhost:9090/spring-petclinic/`  to see the final result
