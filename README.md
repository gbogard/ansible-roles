# Ansible roles

Installing requirements :

```
ansible-galaxy role install -r requirements.yml
```

## Available roles

### Docker-swarm

#### Required groups

- swarm_managers
- swarm_workers

#### Required variables

- advertise_addr (one per host)

### Firewall

Nothing required. Traffic will be enabled on ports 80,443,22 and required ports for Docker Swarm clusters.
The role will also install fail2ban on the system and disable password based authentication.

### Omzsh

Installs Zsh and OMZSH on the server.

### Motd

Configures a nice message of the day on the server.

### Commons

Combines Firewall, Motd, and OMZSH. Installs htop.
