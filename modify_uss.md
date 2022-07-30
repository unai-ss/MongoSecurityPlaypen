## Vagrantfile

line 25

from `centralit.vm.network :private_network, ip: "192.168.14.100"`
to `centralit.vm.network :private_network, ip: "192.168.56.160"`

line 48
from `centralit.vm.network :private_network, ip: "192.168.14.10#{node}"`
to `centralit.vm.network :private_network, ip: "192.168.56.10#{node}"`

line 73
from `centralit.vm.network :private_network, ip: "192.168.14.109"`
to `centralit.vm.network :private_network, ip: "192.168.56.109"`

## os/extrahosts.js

from
```
centralit:192.168.14.100 centralit.vagrant.dev centralit
dbnode1:192.168.14.101 dbnode1.vagrant.dev dbnode1
dbnode2:192.168.14.102 dbnode2.vagrant.dev dbnode2
dbnode3:192.168.14.103 dbnode3.vagrant.dev dbnode3
client:192.168.14.109 client.vagrant.dev client
```

to

```
centralit:192.168.56.100 centralit.vagrant.dev centralit
dbnode1:192.168.56.101 dbnode1.vagrant.dev dbnode1
dbnode2:192.168.56.102 dbnode2.vagrant.dev dbnode2
dbnode3:192.168.56.103 dbnode3.vagrant.dev dbnode3
client:192.168.56.109 client.vagrant.dev client
```
