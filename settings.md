
# Settings


## Command line syntax


Read single setting value:
    
    bitdust set <option name>
    

Write single setting value:

    bitdust set <option name> <new value>


List all available settings and its current values:

    bitdust set list


## List of options
### .DS_Store (undefined)

.DS_Store, default value: None



### api/json-rpc-server/enabled (undefined)

api/json-rpc-server/enabled, default value: None



### api/json-rpc-server/port (undefined)

api/json-rpc-server/port, default value: None



### interface/api/json-rpc-enabled (boolean)

interface/api/json-rpc-enabled, default value: true



### interface/api/json-rpc-port (positive integer)

interface/api/json-rpc-port, default value: 8083



### interface/ftp/enabled (boolean)

interface/ftp/enabled, default value: true



### interface/ftp/port (positive integer)

interface/ftp/port, default value: 8021



### debug level (positive integer)

logs/debug-level, default value: 0

Higher values will produce more log messages.


### enable memory debugger (boolean)

logs/memdebug-enabled, default value: false

Enabled this and go to http://127.0.0.1:[memdebug port number] to watch memory usage.
This feature is disabled at the moment.


### logs/memdebug-port (positive integer)

logs/memdebug-port, default value: 9996



### enable memory profiler (boolean)

logs/memprofile-enabled, default value: false

Use "guppy" package to profile memory usage.
This feature is disabled at the moment.


### enable web logs (boolean)

logs/stream-enabled, default value: false

Enabled this and go to http://127.0.0.1:[logs port number] to browse the program log.
Need to restart the program.


### logs/stream-port (positive integer)

logs/stream-port, default value: 9999



### logs/traffic-enabled (boolean)

logs/traffic-enabled, default value: false



### logs/traffic-port (positive integer)

logs/traffic-port, default value: 9997



### local backups location (folder path)

paths/backups, default value: 

Place for your local backups files.


### donated space location (folder path)

paths/customers, default value: 

Place for your donated space.
All encrypted files, uploaded by other users, will kept here.


### messages location (folder path)

paths/messages, default value: 

Folder to store your private messages.


### receipts location (folder path)

paths/receipts, default value: 

Folder to store financial receipts.


### restored files location (folder path)

paths/restore, default value: 

Location where your restored files should be placed by default.


### betatester (boolean)

personal/betatester, default value: false

Are you agree to participate in the BitDust project testing?
We are going to provide some bonuses to people who help us at this stage.


### personal/email (string)

personal/email, default value: 



### name (string)

personal/name, default value: 

Set your name if you wish.


### nickname (string)

personal/nickname, default value: 

Set your nickname to private messaging.
If you leave this blank your identity address will be used to form a nickname.


### personal/private-key-size (string)

personal/private-key-size, default value: 2048



### surname (string)

personal/surname, default value: 

Set your surname if you wish.


### services/accountant/enabled (boolean)

services/accountant/enabled, default value: false



### enable backups (boolean)

services/backup-db/enabled, default value: true

Enable service "backup-db".


### preferred block size (disk space)

services/backups/block-size, default value: 16 MB

Preferred block size in bytes which used to split the raw data during backup.


### enable backups (boolean)

services/backups/enabled, default value: true

Enable service "Backups".


### keep local copies (boolean)

services/backups/keep-local-copies-enabled, default value: false

Enable this to keep a copy of every new backup on your local HDD as well as on remote machines of your suppliers.
This increases data reliablity, rebuilding performance and decrease network load,
but consumes space on your HDD.
Every one Mb of source data uploaded will consume two Mb on your local HDD.


### maximum block size (disk space)

services/backups/max-block-size, default value: 128 MB

Maximum block size in bytes which used to split the raw data during backup.
The actual block size is calculated depending on size of the particular backup to optimize performance and data storage.
If you plan to do a huge backups - set higher values to increase the speed.


### number of copies (positive integer)

services/backups/max-copies, default value: 2

This value indicates how many copies of each file or directory need to keep on remote machines.
Once a fresh backup of given file or directory were finished - the oldest copy will be removed automatically.
A "0" value means unlimited number of copies, be sure you have enough amount of donated space on remote machines.


### wait suppliers 24 hours (boolean)

services/backups/wait-suppliers-enabled, default value: true

If you disabled storing of local data of your backups but one day a critical amount of your suppliers become unreliable - your data may be lost completely.
Enable this option to wait for 24 hours after finishing any backup and perform a check all of your suppliers before removing the locally backed up data for this copy.


### services/broadcasting/enabled (boolean)

services/broadcasting/enabled, default value: true



### services/broadcasting/max-broadcast-connections (non zero positive integer)

services/broadcasting/max-broadcast-connections, default value: 3



### services/broadcasting/routing-enabled (boolean)

services/broadcasting/routing-enabled, default value: false



### services/contract-chain/enabled (boolean)

services/contract-chain/enabled, default value: false



### services/customer-contracts/enabled (boolean)

services/customer-contracts/enabled, default value: false



### services/customer-patrol/enabled (boolean)

services/customer-patrol/enabled, default value: true



### services/customer-support/enabled (boolean)

services/customer-support/enabled, default value: true



### services/customer/enabled (boolean)

services/customer/enabled, default value: true



### needed space (disk space)

services/customer/needed-space, default value: 1024 MB

How many megabytes you need to store your files?


### number of suppliers (combo box)

services/customer/suppliers-number, default value: 4

Number of remote suppliers which keeps your backups.
You can ser one of the following values: 2, 4, 7, 13, 18, 26, 64.
Right now we have only 16 testing machines in the network, so last three values is not usefull yet.
<font color=red>WARNING!</font> You will lost all your existing backups after changing suppliers number.


### services/data-motion/enabled (boolean)

services/data-motion/enabled, default value: true



### services/employer/enabled (boolean)

services/employer/enabled, default value: true



### services/entangled-dht/enabled (boolean)

services/entangled-dht/enabled, default value: true



### services/gateway/enabled (boolean)

services/gateway/enabled, default value: true



### ebable identity server (boolean)

services/id-server/enabled, default value: false

Enable this to start "id-server" service.


### identity server hostname (string)

services/id-server/host, default value: 

Set a domain name of your machine if you have it.
Otherwise your external IP will be used as a host name.
The host name is used to form a unique IDURL of any hosted identity.
User ID looking more pretty and safe without IP address.


### TCP port number (positive integer)

services/id-server/tcp-port, default value: 6661

A TCP port number to receive user's identity files.


### WEB port number (positive integer)

services/id-server/web-port, default value: 8084

If port 80 is already taken you can start identity server on a different port.


### services/identity-propagate/enabled (boolean)

services/identity-propagate/enabled, default value: true



### services/ip-port-responder/enabled (boolean)

services/ip-port-responder/enabled, default value: true



### services/keys-registry/enabled (boolean)

services/keys-registry/enabled, default value: true



### services/list-files/enabled (boolean)

services/list-files/enabled, default value: true



### services/miner/enabled (boolean)

services/miner/enabled, default value: false



### services/my-ip-port/enabled (boolean)

services/my-ip-port/enabled, default value: true



### services/network/enabled (boolean)

services/network/enabled, default value: true



### services/network/proxy/enabled (boolean)

services/network/proxy/enabled, default value: false



### services/network/proxy/host (string)

services/network/proxy/host, default value: 



### services/network/proxy/password (password)

services/network/proxy/password, default value: 



### services/network/proxy/port (positive integer)

services/network/proxy/port, default value: 



### services/network/proxy/ssl (boolean)

services/network/proxy/ssl, default value: false



### services/network/proxy/username (string)

services/network/proxy/username, default value: 



### incoming bandwidth limit (positive integer)

services/network/receive-limit, default value: 125000000

Limit incoming traffic with a value in bytes per second.
A value of "0" means no incoming limit.


### outgoing bandwidth limit (positive integer)

services/network/send-limit, default value: 12500000

The value in bytes per second to decrease network load.
A value of "0" means no outgoing limit.


### services/nodes-lookup/enabled (boolean)

services/nodes-lookup/enabled, default value: true



### services/p2p-hookups/enabled (boolean)

services/p2p-hookups/enabled, default value: true



### services/private-messages/enabled (boolean)

services/private-messages/enabled, default value: false



### services/proxy-server/current-routes (text)

services/proxy-server/current-routes, default value: {}



### services/proxy-server/enabled (boolean)

services/proxy-server/enabled, default value: false



### services/proxy-server/routes-limit (positive integer)

services/proxy-server/routes-limit, default value: 10



### services/proxy-transport/current-router (string)

services/proxy-transport/current-router, default value: 



### services/proxy-transport/enabled (boolean)

services/proxy-transport/enabled, default value: false



### services/proxy-transport/my-original-identity (text)

services/proxy-transport/my-original-identity, default value: 



### services/proxy-transport/preferred-routers (text)

services/proxy-transport/preferred-routers, default value: 



### services/proxy-transport/priority (positive integer)

services/proxy-transport/priority, default value: 30



### services/proxy-transport/receiving-enabled (boolean)

services/proxy-transport/receiving-enabled, default value: false



### services/proxy-transport/router-lifetime-seconds (positive integer)

services/proxy-transport/router-lifetime-seconds, default value: 600



### services/proxy-transport/sending-enabled (boolean)

services/proxy-transport/sending-enabled, default value: true



### services/rebuilding/enabled (boolean)

services/rebuilding/enabled, default value: true



### services/restores/enabled (boolean)

services/restores/enabled, default value: true



### services/supplier-contracts/enabled (boolean)

services/supplier-contracts/enabled, default value: false



### services/supplier/donated-space (disk space)

services/supplier/donated-space, default value: 8 GB



### services/supplier/enabled (boolean)

services/supplier/enabled, default value: true



### services/tcp-connections/enabled (boolean)

services/tcp-connections/enabled, default value: true



### tcp port number (positive integer)

services/tcp-connections/tcp-port, default value: 7771

Enter the TCP port number, it will be used to connect with your machine by other users.


### UPnP enable (boolean)

services/tcp-connections/upnp-enabled, default value: true

Enable this if you want to perform checking of UPnP devices to configure port forwarding automatically.


### enable tcp-transport service (boolean)

services/tcp-transport/enabled, default value: true

Enable "TCP-transport" service.


### services/tcp-transport/priority (positive integer)

services/tcp-transport/priority, default value: 10



### enable tcp receiving (boolean)

services/tcp-transport/receiving-enabled, default value: true

Disable this if you do not want to use TCP-transport for receiving packets from other users.


### enable tcp sending (boolean)

services/tcp-transport/sending-enabled, default value: true

Disable this if you do not want to use TCP-transport for sending packets to other users.


### services/udp-datagrams/enabled (boolean)

services/udp-datagrams/enabled, default value: true



### udp port number (positive integer)

services/udp-datagrams/udp-port, default value: 8882

Set a UDP port for sending and receiving UDP datagrams.


### enable udp-transport service (boolean)

services/udp-transport/enabled, default value: true

Enable "UDP-transport" service.


### services/udp-transport/priority (positive integer)

services/udp-transport/priority, default value: 20



### enable udp receiving (boolean)

services/udp-transport/receiving-enabled, default value: true

Disable this if you do not want to use UDP-transport for receiving packets from other users.


### enable udp sending (boolean)

services/udp-transport/sending-enabled, default value: true

Disable this if you do not want to use UDP-transport for sending packets to other users.



