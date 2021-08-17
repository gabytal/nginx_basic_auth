# this is a NGINX server proxy that simply require user & password in order to pass to proxy server

# first,install the apache2 tools to generate new password file
sudo apt-get install apache2-utils

# generate the file
htpasswd -c /etc/nginx/.htpasswd admin

# restart NGINX
systemctl restart nginx
