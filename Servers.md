# <img src="configure-sm.png" width=30></img>Configure ownCloud Servers
Once you have installed the server, open the ownCloud Admin panel and complete your server configuration. You can configure several features, including:

- Security
- File handling
- Sharing
- Cron jobs
- Email server

## Add a Trusted Domain

Enable users to connect to your ownCloud server using a specified domain. You can whitelist your server address in the `config.php` file. 

### Example
This example shows how to add `myserver.example.com` with port `8080` to the whitelist.

1. Open `config.php`.
2. Add your server and port address top the **trusted_domains** paramerter:

```
'trusted_domains' => [
   '192.168.1.50:8080',
],
```

Users can now connect to the ownCloud server using this server and port address. For more infromation, see [Server Access](access.md). 

## Related Information
- [ownCloud Installation](install.md)
- [User Management] (user.md)
- [Server Access](access.md)
- [ownCloud Quick Start](introduction.md)