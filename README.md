# terraform-docker-jenkins-cicd
how to build a Jenkins Docker image that has Docker and Terraform baked in. and play with ci/cd

For jenkins file 1
====================================

In the Jenkins dashboard, click New Item Enter an item name of PipelinePart1, and select Pipeline. Click Ok.

Check the box for This project is parameterized. Click Add Parameter and select Choice Parameter. Give it a Name of action. For Choices, enter Deploy and Destroy, and make sure they are on separate lines. Enter The action that will be executed as the Description.

Click Add Parameter and select Choice Parameter again. This time, name it image_name. Enter ghost:latest and ghost:alpine in the Choices box, making sure they are on separate lines. Enter The image Ghost Blog will deploy as a Description.

Click Add Parameter a third time, and select String Parameter. Give it a Name of ext_port. Set the Default Value to 80. Enter The Public Port as the Description.


For jenkins file 2
====================================

In the Jenkins dashboard, click New Item Enter an item name of PipelinePart2, and select Pipeline. Click Ok.

Check the box for This project is parameterized. Click Add Parameter and select Choice Parameter. Give it a Name of action. For Choices, enter Deploy and Destroy, and make sure they are on separate lines. Enter The action that will be executed as the Description.

Click Add Parameter and select Choice Parameter again. This time, name it image_name. Enter ghost:latest and ghost:alpine in the Choices box, making sure they are on separate lines. Enter The image Ghost Blog will deploy as a Description.

Click Add Parameter a third time, and select String Parameter. Give it a Name of ghost_ext_port. Set the Default Value to 80. Enter The Public Port as the Description.
The add script of jenkinsfile2

For jenkins file 2
====================================
In the Jenkins dashboard, click New Item Enter an item name of PipelinePart3, and select Pipeline. Click Ok.

Check the box for This project is parameterized. Click Add Parameter and select Choice Parameter. Give it a Name of action. For Choices, enter Deploy and Destroy, and make sure they are on separate lines. Enter The action that will be executed as the Description.

Click Add Parameter and select String Parameter. For the name, enter mysql_root_password.. Enter P4ssW0rd0! in the Default Value box. Enter MySQL root password. as a Description.

For the second parameter, click Add Parameter once more and select String Parameter. For the name, enter mysql_user_password.. Enter paSsw0rd0! in the Default Value box. Enter MySQL user password. as a Description.

Down in the Pipeline section, give a Definition of Pipeline script from jenkinsfile3
