# Firewall Configuration

## 1. Allow SSH

The following command allows SSH connections so administrators can remotely manage the server.

```bash
sudo ufw allow ssh
```

## 2. Set the Default Firewall Policies

These commands block incoming traffic by default while allowing outgoing traffic.

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

## 3. Enable the Firewall

This command activates the UFW firewall.

```bash
sudo ufw enable
```

To verify the firewall status, use:

```bash
sudo ufw status verbose
```

## 4. Allow Port 8080

This command allows incoming TCP traffic on port 8080 so users can access the Nginx web application.

```bash
sudo ufw allow 8080/tcp
```

To check the numbered firewall rules, use:

```bash
sudo ufw status numbered
```

## 5. Importance of Allowing SSH First

If `sudo ufw enable` is run before `sudo ufw allow ssh`, SSH connections may be blocked by the default deny incoming policy, potentially locking remote administrators out of the server.
