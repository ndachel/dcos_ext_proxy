# dcos_ext_proxy
Expose load balanced marathon services externally via haproxy

- Checks task list from Marathon REST API
- Checks app balace config from etcd
- Rewrites haproxy.cfg
- If DIFF, restart haproxy with new config

Also, this is intended to be built with DCOS Velocity (Jenkins->Git->Mesos Jenkins Slave->Docker Build->Marathon deploy)
