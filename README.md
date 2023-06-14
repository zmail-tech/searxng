# searxng
Docker compose setup for a searxng instance with custom logo and redis

#Prerequisites
This docker-compose file relies on having the jwilder/nginx-proxy setup already running on your server.
There is an example of what I run on my github page

Once the nginx proxy with letsencrypt is setup to run this container run

# Add Custon Branding (Optional)
To add your own custom logo and favicon uncomment the appropriate lines in the compose file and supply the files in the project directory to be mounted in

#Environment File
There is a .env file in this directory. Please edit the file with the URL you need to use (without specifying https)
Enter your email in the appropriate location too in the .env file

#To run this compose file
docker-compose up -d

Assuming your nginx proxy and letsencrypt companion is setup you can access your searxng instance at https://your.domain.com that you supplied in the .env file
