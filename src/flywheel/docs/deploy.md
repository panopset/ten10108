

Copy up your server block file and install your certs.


    ./ds.sh
    ssh prod
    sudo ln -s /etc/nginx/sites-available/<your domain> /etc/nginx/sites-enabled/
    sudo nginx -t
    sudo systemctl restart nginx
    sudo certbot --nginx -d <your domain> -d www.<your domain>

... and take option 2 to redirect all http to https.

# Deploy ten10108.com...

## ... to your local development nginx server:
    

    ./dl.sh


## ... to your production server:


    ./dp.sh



