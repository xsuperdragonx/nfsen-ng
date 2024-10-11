# nfsen-ng
nfsen-ng docker compose and config

To use nfsen-ng:
1. Prepare the exporter from Netflow, Sflow and let it send data to the port of nfsen-dump container
2. Clone this git repo to your machine
3. Update the flow at file sources.conf
4. Each flow will use one port, you need to open each port to outside for this to work
5. Run:
   
   docker compose up -d
   
   docker exec nfsen-ng ln -s /usr/local/bin/nfdump /usr/bin/nfdump
7. Wait a bit and access the web at  http://your-server-ip:81 
