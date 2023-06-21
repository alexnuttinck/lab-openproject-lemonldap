# lemonldap-openproject

Run OpenProject with LemonLDAP::NG as authentication provider (SSO).

## Requirements

Update your `/etc/hosts` file with the following entries:

```
127.0.0.1 auth.example.local
127.0.0.1 manager.example.local
127.0.0.1 handler.example.local
127.0.0.1 openproject.example.local
```

## Usage

```bash 
docker-compose -f docker-compose-lemonldap.yml -f docker-compose-openproject.yml up -d
```

## Configuration

### LemonLDAP

The default login is `dwho` and the default password is `dwho`.

Go in the WebSSO tab.

### OpenProject

The default login is `admin` and the default password is `admin`.

Go in Administration > Authentication > OpenID providers.

Check the documentation: https://www.openproject.org/docs/installation-and-operations/misc/custom-openid-connect-providers/






