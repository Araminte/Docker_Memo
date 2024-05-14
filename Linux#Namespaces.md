<div align="center">
    <em>" Namespaces are a feature of the Linux kernel that partition kernel resources such that one set of processes sees one set of resources, while another set of processes sees a different set of resources. The feature works by having the same namespace for a set of resources and processes, but those namespaces refer to distinct resources. Resources may exist in multiple spaces. Examples of such resources are process IDs, host-names, user IDs, file names, some names associated with network access, and Inter-process communication.
    Namespaces are a fundamental aspect of containers in Linux. The term "namespace" is often used to denote a specific type of namespace (e.g. process ID) as well as for a particular space of names.
    A Linux system begins with a single namespace of each type, used by all processes. Processes can create additional namespaces and can also join different namespaces."</em><br><br>
</div>


```bash
hostname 
#[hostname1]
unshare --uts
hostname 
#[hostname1]
hostname newname
hostname 
#[newname]
```
In an other terminal :

```bash
hostname
#[hostname1]
```