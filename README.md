# Unifi Network Server Service

Unifi Network Server is a self-hosted service for manage your unifi devices.

For more information click [here][UI Help Site].

## How to install and run

- First make a copy of the ".env.example" file and rename it to ".env";
- Fill the variables in the .env file and make sure the ports number you're using is not being used on another services;

After that you can run the command:

`docker-compose up -d`

If everything runs fine you can access the webui site with machine ip and the port you chosen. Examples (filling the $WEBUI_PORT with `8443`):

- 127.0.0.1:8443;
- localhost:8443;
- YOUR_COMPUTER_IP:8443;

## Device Adoption

Follow the guide described on LinuxServer site [here][LinuxServer Device Adoption]

## Database

This compose file is configured to use an external MongoDB database, but if you want, you can add a MongoDB image. Just follow the guide at [LinuxServer][LinuxServer MongoDB]

[UI Help Site]: https://docs.linuxserver.io/images/docker-unifi-network-application/#device-adoption

[LinuxServer Device Adoption]: https://github.com/linuxserver/docker-unifi-network-application?tab=readme-ov-file#device-adoption

[LinuxServer MongoDB]: https://github.com/linuxserver/docker-unifi-network-application?tab=readme-ov-file#setting-up-your-external-database
