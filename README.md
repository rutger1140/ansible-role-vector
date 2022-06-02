# Ansible Vector for Ubuntu with Logtail

Configures Vector with Ansible for nginx, fail2ban and haproxy. Logging is piped into logtail.com.

## Log files

Currently these log files are ingested:

- nginx access + error logs (`/srv/www/domain.com/logs/*.log`)
- auth log (`/var/log/auth.log`)
- fail2ban log (`/var/log/fail2ban.log`)
- haproxy log (`/var/log/haproxy.log`)

## Configuration

- `vector_logtail_bearer_token` - add the 'Source token' from Logtail.com
- `vector_nginx_logs_path` - set the path to your nginx logs
