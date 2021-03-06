# Minecraft on Akash

## Deploying Minecraft on the Decentralised Cloud

This repository will show you how to deploy different types of Minecraft servers on Akash.

***

### Getting Started

You will need to choose a way to deploy to Akash. They have several deployment guides in their documentation. https://docs.akash.network/

You can currently pick from:

- Akash Deploy UI (Web App) - https://docs.akash.network/guides/deploy
- Akashlytics Deploy (Desktop App) - https://docs.akash.network/guides/app
- Akash Command (Cli) - https://docs.akash.network/guides/command

You will also need to create an AKT wallet. You can do this with any of the methods above or by using Keplr wallet or Cosmostation. (There is information about this in the Akash Documents too.)
https://docs.akash.network/guides/wallet

I have added some more examples with the newest version of Akash CLI 0.14.0 (https://docs.akash.network/release-notes/v0.14.0). 

This makes it easier to access the Deployment Shell (CLI) and manage your server. It also allows you to copy files from your container to a local instance.

In my examples, I have added automatic backups to Filebase and used MCrcon to manage the server as well.

***

### Pick a Minecraft Docker Image

There are plenty of Minecraft Docker Images to choose from. 

You can find quite a few at https://hub.docker.com/ 

Just type Minecraft in the search bar and you will see many results. 

You can also create your own Minecraft Docker Image with a custom Dockerfile or

You can use my image by pulling moonbys/minecraft:master

***

## Deploy Steps

- Create your own Minecraft Docker Image or use one from the examples folder
- Create your own deploy.yaml file or use one from the examples folder (change the Docker Image and settings to your needs)
- Use your selected Akash deploy method to send your selected deploy.yaml
- Log in to your Minecraft server and have fun

***

### Notes

- All of the deploy.yaml files in the examples folder include RCON setup, so that you can interact with your server (You will need mcrcon https://github.com/Tiiffi/mcrcon) You can also delete the RCON lines and port, if you do not plan to use this. 
- Some of the example servers include auto backups to Filebase.com

