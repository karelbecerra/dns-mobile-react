# HTTPS React Local Deb Env Proxy
Simple SSL HTTP proxy using a self-signed certificate. Intended for local development only.

# Install
> npm install -g local-ssl-proxy

# Run
To start a proxy from port 3001 to 3000 run:

> local-ssl-proxy --source 3001 --target 3000

Start your web server on the target port (3000 in the example) and navigate to https://localhost:<target-port> (https://localhost:3001 in the example). You'll get a warning because the certificate is self-signed, this is safe to ignore during development.


