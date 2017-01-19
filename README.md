
emq-recon
=========

Recon debug/optimize plugin

Load the Plugin
---------------

```
./bin/emqttd_ctl plugins load emq_recon
```

Commands
--------

```
./bin/emqttd_ctl recon

recon memory                            #recon_alloc:memory/2
recon allocated                         #recon_alloc:memory(allocated_types, current|max)
recon bin_leak                          #recon:bin_leak(100)
recon node_stats                        #recon:node_stats(10, 1000)
recon remote_load Mod                   #recon:remote_load(Mod)
```

GC
--

When the plugin is loaded, global GC will run periodically.

License
-------

Apache License Version 2.0

Author
------

Feng Lee <feng@emqtt.io>

