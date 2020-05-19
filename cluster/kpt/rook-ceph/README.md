rook-ceph
==================================================

# NAME

  Rook operator for Ceph

# SYNOPSIS

`kubectl apply -k rook-ceph/instance`

# Description

kpt rook-сeph package

## Get package

`kpt pkg get https://github.com/denisok/rook/cluster/kpt/rook-ceph@rook-ceph/v1.3.3 rook-ceph`

## Configuration

### Check current configuration

`kpt cfg list-setters rook-ceph`

### Set configuration

`kpt cfg set rook-ceph cephcsi-img-path registry.suse.de/devel/storage/7.0/containers/ses/7/cephcsi/cephcsi`

`kpt cfg set rook-ceph cephcsi-img-tag 2.0.0`

## Customizations

Customize deployment with "kustomize" inside `instance`  directory

## Apply the package to a cluster

`kubectl apply -k rook-ceph/instance`

## Update

https://googlecontainertools.github.io/kpt/guides/consumer/update/

# SEE ALSO

https://googlecontainertools.github.io/kpt/guides/consumer/
