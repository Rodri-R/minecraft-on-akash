- Download Bukkit/Spigot plugin jars, such as WorldEdit and place them in this directory. 
- At image build time the COPY step will place those jars in /plugins. 
- At container startup, the contents of /plugins are sync'ed into /data/plugins for use with Bukkit/Spigot/Paper server types.
- Have fun & enjoy