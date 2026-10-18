# Firewall Configuration

## Commands Used

### 1. Allow SSH
```bash
sudo ufw allow ssh
```

### 2. Set the Default Deny Policy
```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

### 3. Enable the Firewall
```bash
sudo ufw enable
```

### 4. Allow Port 8080
```bash
sudo ufw allow 8080/tcp
```

### 5. Verify Firewall Rules
```bash
sudo ufw status verbose
sudo ufw status numbered
```

## SSH Security Warning

If I run `sudo ufw enable` before `sudo ufw allow ssh`, incoming SSH connections may be blocked, potentially locking me out of remote server administration.

## Summary

UFW was configured to deny incoming traffic by default while allowing outgoing traffic, SSH access, and TCP port 8080 for the web application.
