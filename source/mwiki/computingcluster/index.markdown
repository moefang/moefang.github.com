---
layout: page
title: "Use Computing Linux Cluster"
date: 2012-09-06 22:57
sidebar: false
comments: false
sharing: true
footer: false
---
### Login the computing cluster

``` sh
ssh mfang@orion0.eng.uts.edu.au
```
The `mfang` is a user id and `orion0` is one of vitual computer. Then I should     input the password.
### Get the list of available nodes
View the status of all clusters.
``` sh
cnode
```
View the status of one cluster, for example orion.
``` sh
cnode orion
```
### Jump to another vitual computer or connect to a node
``` sh
ssh orion4
```
### Logout
``` sh
exit
```
