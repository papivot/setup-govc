# Setup GOVC.

create `~/.govcenv`

Sample info - 

```shell
export GOVC_URL=my_vcenter_fqdn
export GOVC_HOST=my_esxi_host_fqdn_if_i_want_to_reference_it
export GOVC_USERNAME="administrator@vsphere.local"
export GOVC_PASSWORD="mypassword"
export GOVC_INSECURE=true
export GOVC_DATACENTER=Datacenter
export GOVC_DATASTORE=LUN01
export GOVC_NETWORK="VM Network"
export GOVC_RESOURCE_POOL=
```

```shell
wget https://github.com/vmware/govmomi/releases/download/v0.22.1/govc_linux_amd64.gz
gzip -d govc_linux_amd64.gz
chmod +x govc_linux_amd64
sudo mv govc_linux_amd64 /usr/local/bin/govc
source ~/.govcenv
govc env 
```
