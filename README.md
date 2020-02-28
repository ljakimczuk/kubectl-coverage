# The Kubectl Coverage plugin

The kubectl-coverage plugin calculates distribution of Pods, from a given namespace or all namespaces, across all instances.

## Getting Started

These instructions will get you a copy of this plugin up and running.

### Prerequisites

The plugins requires tools listed below to work correctly:

```
parallel >= 20161222
```

### Installing

To install the plugin, execute the following command:

```
sudo curl -L https://github.com/ljakimczuk/kubectl-coverage/raw/master/bin/kubectl-coverage -o /usr/local/bin/kubectl-coverage
sudo chmod a+x /usr/local/bin/kubectl-coverage
```

### Usage

In order to calculate the coverage run the plugin without any parameters or pass a namespace name to it:

```
$ kubectl coverage
node1  20.00%
node2  20.00%
node3  60.00%

$ kubectl coverage default
node1  100.00%
```
