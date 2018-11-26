# ![](../images/configure-sm.png) Configure ownCloud Servers
Once you have installed the server, open the ownCloud Admin panel and complete your server configuration. You can configure several features, including:

- Security
- File handling
- Sharing
- Cron jobs
- Email server

For more configuration information, see the latest [Server Administration Manual](https://doc.owncloud.org/server/latest/admin_manual/configuration/).

## Add a Trusted Domain

Enable users to connect to your ownCloud server using a specified domain. Whitelist your server address in the `config.php` file. 

### Example
This example shows how to add the IP address `192.168.1.50` with port `8080` to the whitelist.

1. Open `config.php`.
2. Add your server and port address top the **trusted_domains** parameter:

```
'trusted_domains' => [
   '192.168.1.50:8080',
],
```

Users can now connect to the ownCloud server using this server and port address. For more information, see [Server Access](access.md). 

## Related Information
* [Install ownCloud Servers](install.md)
* [Add User Accounts](User.md)
* [Access ownCloud Servers](access.md) 
* [ownCloud Quick Start Guide](../README.md)