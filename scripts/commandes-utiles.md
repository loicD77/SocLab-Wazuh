# Commandes utiles

## Vérifier les agents
```bash
sudo /var/ossec/bin/agent_control -l
```

## Vérifier les services
```bash
sudo systemctl status wazuh-manager
sudo systemctl status wazuh-dashboard
sudo systemctl status wazuh-agent
```

## Réseau
```bash
ip addr
ip route
ping -c 4 192.168.8.149
```

## Nmap
```bash
nmap -A 192.168.8.149
nmap -sV 192.168.8.149
```

## Journaux
```bash
sudo journalctl -u wazuh-agent -n 50 --no-pager
```

## Redémarrer
```bash
sudo systemctl restart wazuh-manager
sudo systemctl restart wazuh-dashboard
sudo systemctl restart wazuh-agent
```
