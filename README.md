# My web server configuration

## Start node application with pm2

    $ pm2 start npm -- start

## Using SSL with multiple domains

    $ certbot certonly --manual --preferred-challenges dns --server https://acme-v02.api.letsencrypt.org/directory --manual-public-ip-logging-ok -d '*.<your.domain>' -d <your.domain>
    
With my domain

    $ certbot certonly --manual --preferred-challenges dns --server https://acme-v02.api.letsencrypt.org/directory --manual-public-ip-logging-ok -d '*.alexandre-hublau.com' -d alexandre-hublau.com

### More info:

https://dev.to/nabbisen/let-s-encrypt-wildcard-certificate-with-certbot-plo
