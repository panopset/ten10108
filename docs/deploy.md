[home](../README.md)

Copy up your server block file, make it available, and test the config.


    ./ds.sh
    ssh prod
    sudo ln -s /etc/nginx/sites-available/<your domain> /etc/nginx/sites-enabled/
    sudo nginx -t

# Deploy ten10108.com...

## ... to your local development nginx server:
    

    ./dl.sh


## ... to your production server:


    ./dp.sh




