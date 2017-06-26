# HTTPS with client certificate authentication

To protect your openHAB instance in the public Internet network we can use client authenticate with SSL certificate feature.

In order to prepare environment to work with this feature we must to do some below steps:

## Own Certificate Authority

sudo openhabian-config

>> openhab related >> reverse proxy

## Load balancer with client certificate verification
TODO

## Client configuration

this works with setup via openhabian-config

sudo -s

openssl pkcs12 -export -out /etc/ssl/certificate.pfx -inkey /etc/ssl/certs/openhab.key -in /etc/ssl/certs/openhab.crt

password which will be needed when adding certificate to android device.

You can download certificate via any SCP client(windows WinSCP) /etc/ssl/certificate.pfx
certificate.pfx can be used for android authentication.

credits
https://www.ssl.com/how-to/create-a-pfx-p12-certificate-file-using-openssl/
