---
---
**General Option**

{{< truetable >}}
| Settings | Description |
|----------|-------------|
| **Database Path** | Sets the database information stored in the path. The path must be writable even if the pool is read only. |
{{< /truetable >}}

**Access**

{{< truetable >}}
| Settings | Description |
|----------|-------------|
| **Guest Account** | Select an account to use for guest access. This account must have permissions to the shared pool or dataset. The privileges given to this user are also available to any client connecting to the guest service. This user must exist in the password file, but does not require a valid login. The root user cannot be used as guest account. |
| **Guest Access** | Select to disable the password prompt that displays before clients access AFP shares. |
| **Max Connections** | Maximum number of simultaneous connections permitted via AFP. The default limit is **50**. |
| **Chmod Request** | Indicates how to handle access control lists. Select **Ignore** to ignore requests and give the parent directory ACL inheritance full control over new items. Select **Preserve** to preserves ZFS ACEs for named users and groups or the POSIX ACL group mask. Use **Simple*8 to set to chmod() as requested without any extra steps. |
| **Map ACLs** | Select mapping of permissions for authenticated users. Select **Rights (default, Unix-style permissions)**, **None**, or **Mode (ACLs)**. |
{{< /truetable >}}

**Other Options**

{{< truetable >}}
| Settings | Description |
|----------|-------------|
| **Log Level** | Record AFP service messages up to the specified log level in the system log. By default, severe and warning level messages are logged. |
| **Bind Interfaces** | Specify the IP addresses to listen for AFP connections. Leave blank to bind to all available IPs. If none are specified, advertise the first IP address of the system, but listen for any incoming request. |
| **Global Auxiliary** | Additional [afp.conf(5)](http://netatalk.sourceforge.net/3.0/htmldocs/afp.conf.5.html) parameters. |
{{< /truetable >}}
