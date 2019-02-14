# wireguard-install

```
curl -O https://raw.githubusercontent.com/LiveChief/wireguard-install/master/wireguard-install.sh 
bash wireguard-install.sh
```


Install WireGuard and reboot your computer:
```
sudo add-apt-repository ppa:wireguard/wireguard -y && sudo apt update && sudo apt install wireguard resolvconf -y
sudo reboot
Copy the file /root/client-wg0.conf from a remote server to your local PC path /etc/wireguard/wg0.conf
sudo systemctl start wg-quick@wg0.service
```

To show VPN status, run sudo wg show.
