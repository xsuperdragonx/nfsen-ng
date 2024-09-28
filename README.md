# nfsen-ng
nfsen-ng docker compose and config

To use nfsen-ng:
1. Prepare the exporter from Netflow, Sflow and let it send data to the port of nfsen-dump container
2. Clone this git repo to your machine
3. Run:
   docker compose up -d
   docker exec nfsen-ng-nfdump ln -s /usr/local/bin/nfdump /usr/bin/nfdump
4. Wait a bit and access the web at  http://your-server-ip:81 
