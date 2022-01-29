# vowable
                                               *Lightweight Steam client framework for node*


Vowable is a lightweight Steam client for managing multiple account and provides unified API for writing custom extensions. Vowable takes care of the basic stuff such as maintaining connection, logging in and exposes simple API which allows custom plugins to extend its behaviour.

**Client**
*Vowable provides a very simple automated client. This client uses node-steam to connect to Steam servers.*

Vowable provides several key features;
`handles log in process, including auth codes and sentry files
provides API for plugins
provides unified logging interface
provides a bunch of built-in plugins to make your life easier
Everything else needs to be programmed separately using plugin system.`


**Plugins**
Plugins are self-contained code snippets which extend Vapor's behaviour.

Plugins have:

access to active Steam client instance and handlers
access to Steam's enums
They can:

create and login-to accounts
listen to custom events
customize their own  settings
store and copy data
...
Plugins are entirely event driven, there are no hard dependencies. Each plugin can emit an event and any plugin may register a callback for such event.
This architecture allows your code to be modular and decoupled.

Within this script there will be a local hosted website ran where you can manage and access all the accounts to log-into. It's all client-sided meaning none of your information gets stored anywhere else than your own computer. 


