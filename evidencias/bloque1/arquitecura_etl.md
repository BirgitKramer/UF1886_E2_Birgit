# Arquitectura

### Contenedores activos


##### comando
```
 docker ps --format "table {{.Names}}\t{{.Image}}\t{{.Ports}}\{{.Status}}"
```
```
NAMES         IMAGE                PORTS\STATUS
odoo.18       odoo:18.0            0.0.0.0:8001->8069/tcp, [::]:8001->8069/tcp, 0.0.0.0:8002->8072/tcp, [::]:8002->8072/tcp\Up 30 minutes
postgres.db   postgres:16-alpine   0.0.0.0:5432->5432/tcp, [::]:5432->5432/tcp\Up 30 minutes
```

### Network
```
NETWORK ID     NAME                         DRIVER    SCOPE
eb07528d75ca   uf1886_e2_birgit_default     bridge    local
```
### Volumen
```
local     uf1886_e2_birgit_odoo-db-data
local     uf1886_e2_birgit_odoo-web-data
```
### Recursos del host
```
DeviceID Name                                           Caption                               MaxClockSpeed SocketDesig
                                                                                                            nation
-------- ----                                           -------                               ------------- -----------
CPU0     11th Gen Intel(R) Core(TM) i5-1135G7 @ 2.40GHz Intel64 Family 6 Model 140 Stepping 1 2419          U3E1

TotalVisibleMemorySize FreePhysicalMemory
---------------------- ------------------
              16507816            6841180

```