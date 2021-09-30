# Shepherd Pools 

This folder contains the Shepherd pool definition files.

To use Shepherd, you must first install the `sheepctl` CLI tool. You MUST be connected to the VPN to use Shepherd.

A mored detailed guide to getting started with Shepherd and TKG test pools can be found here: https://confluence.eng.vmware.com/pages/viewpage.action?spaceKey=TKG&title=TKG+Testbed

## Installing sheepctl

###  on Linux
```
wget http://files.pks.eng.vmware.com/ci/artifacts/shepherd/latest/sheepctl-linux-amd64
cp sheepctl-linux-amd64 /usr/local/bin/
chmod +x /usr/local/bin/sheepctl
```
###  on MacOS
```
brew tap vmware/internal git@gitlab.eng.vmware.com:homebrew/internal.git
brew install sheepctl
```

## Creating/updating pools

To create a pool run:

```
sheepctl pool create -n spring-cloud-dataflow -f POOL_DEFINTION.json
```

To update a pool run:
```
sheepctl pool update -n spring-cloud-dataflow -f POOL_DEFINTION.json
```
