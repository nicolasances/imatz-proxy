README 

To use NGINX with the certificates that have been released by Let's encrypt (https://letsencrypt.org/) you have 
to mount the certificates volume on /certificates: 

docker run -d -p 443:443 -v /etc/letsencrypt/archive/imatz.info:/certificates --name imatz-proxy nicolasances/imatz-proxy