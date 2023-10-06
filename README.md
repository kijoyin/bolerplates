# Bolerplates

## Home Lab
### Docker Swarm
Open all ports mentioned in the below article 
https://www.digitalocean.com/community/tutorials/how-to-configure-the-linux-firewall-for-docker-swarm-on-ubuntu-16-04
FOr open suse 
```
sudo firewall-cmd --zone=public --add-port=**<PORT>**/tcp
sudo firewall-cmd --runtime-to-permanent
```
#### Ports opened for doecker swarm to communicate
```
sudo firewall-cmd --zone=public --add-port=22/tcp
sudo firewall-cmd --runtime-to-permanent
sudo firewall-cmd --zone=public --add-port=2376/tcp
sudo firewall-cmd --runtime-to-permanent
sudo firewall-cmd --zone=public --add-port=2377/tcp
sudo firewall-cmd --runtime-to-permanent
sudo firewall-cmd --zone=public --add-port=7946/tcp
sudo firewall-cmd --runtime-to-permanent
sudo firewall-cmd --zone=public --add-port=7946/udp
sudo firewall-cmd --runtime-to-permanent
sudo firewall-cmd --zone=public --add-port=4789/udp
sudo firewall-cmd --runtime-to-permanent
```
### Traefik in Docker Swarm
https://dockerswarm.rocks/traefik/
