# My web server configuration

## Using SSL with multiple domains

  certbot certonly --manual --preferred-challenges dns --server https://acme-v02.api.letsencrypt.org/directory --manual-public-ip-logging-ok -d '*.<your.domain>' -d <your.domain>

More info:

(https://dev.to/nabbisen/let-s-encrypt-wildcard-certificate-with-certbot-plo)[https://dev.to/nabbisen/let-s-encrypt-wildcard-certificate-with-certbot-plo]
