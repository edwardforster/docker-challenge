# docker-challenge
Docker challenge for Blackbook.ai

To run input the command "docker-compose up -d" while in the directory of the yml file, and "docker-compose down" to shut down the containers.
To view the wordpress output enter "http://localhost:9090" into the url bar of your browser. To make entries through wordpress enter "http://localhost:9090/wp-admin/" into
the url bar of your browser which will prompt for credentials. The username is "edward" and the password is "pass".

A wordpress container has been used as a frontend and mysql as a backend for this challenge. The two containers communicate with eachother via MySQL authentication through
the appropriate opened ports. Bind mounts have been utilised to store the details required for the Wordpress and MySQL containers rather than volumes, to ease the ability to
share the files to another host.
