# Linux: Control Groups

cgroups are a kernel feature that allows users to group processes and control, limit, and monitor the system resources those groups can use

* Arranged hierarchically where child groups inherit or subdivide limits from their parents
* Exposed via a virtual filesystem by the kernel where each directory corresponds to a cgroup
* Every process belongs to at least one cgroup

<br>

# Controllers

Controllers in cgroups are kernel modules that enforce specific resources limits, accounting, and prioritization rules for processes within a cgroup

<br>

# cgroup Versions

## cgroup v1

* Multiple hierarchies (one per controller)
* Separate mounts per controller (`/sys/fs/cgroup/cpu`)

## cgroup v2

* Single unified hierarchy
* Single mount point (`sys/fs/cgroup`)

<br>

# cgroupfs