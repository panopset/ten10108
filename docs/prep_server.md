[home](../README.md)

## DigitalOcean Server Preparation

On a [digitalocean](https://digitalocean.com) [nginx server set up with server blocks](https://www.digitalocean.com/community/tutorials/how-to-install-nginx-on-ubuntu-20-04) and [letsencrypt](https://www.digitalocean.com/community/tutorials/how-to-secure-nginx-with-let-s-encrypt-on-ubuntu-20-04):

Replace <your domain> with your domain name, for example ten10108.com:

    mkdir -p /var/www/<your domain>/html
    sudo chown $USER /etc/nginx/sites-available

