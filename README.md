Before you run a playbook create a VM and specify its external IP address in ``hosts`` file.  

To install and configure dnsmasq:
```
ansible-playbook --skip-tags "uninstall" -i hosts dnsmasq.yaml -vv
```
To uninstall dnsmasq:
```
ansible-playbook --tags "uninstall" -i hosts dnsmasq.yaml -vv
```
To check syntax before running:
```
ansible-playbook dnsmasq.yaml  --syntax-check
```
