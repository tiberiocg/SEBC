-List the cloud provider you are using (AWS, GCE, Azure, other)
aws


-List the nodes you are using by IP address and name
hostname ip-172-31-33-209.us-west-2.compute.internal
internal ip 172-31-33-209
external ip 52.41.64.217

hostname ip-172-31-37-222.us-west-2.compute.internal
internal ip 172-31-37-222
external ip 52.10.97.0

hostname ip-172-31-43-23.us-west-2.compute.internal
internal ip 172-31-43-23
external ip 34.209.243.212

hostname ip-172-31-43-220.us-west-2.compute.internal
internal ip 172-31-43-220
external ip 34.210.34.78

hostname ip-172-31-34-114.us-west-2.compute.internal
internal ip 172-31-34-114
external ip 52.27.63.232


-Demonstrate the disk capacity available on each node is >= 30 GB
[ec2-user@ip-172-31-33-209 yum.repos.d]$ hostname -f
ip-172-31-33-209.us-west-2.compute.internal
[ec2-user@ip-172-31-33-209 yum.repos.d]$
[ec2-user@ip-172-31-33-209 yum.repos.d]$
[ec2-user@ip-172-31-33-209 yum.repos.d]$  df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2       40G  2.1G   38G   6% /
devtmpfs        7.3G     0  7.3G   0% /dev
tmpfs           7.2G     0  7.2G   0% /dev/shm
tmpfs           7.2G   25M  7.2G   1% /run
tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
tmpfs           1.5G     0  1.5G   0% /run/user/1000
/dev/xvdb        40G   33M   40G   1% /data
tmpfs           1.5G     0  1.5G   0% /run/user/0

[ec2-user@ip-172-31-37-222 yum.repos.d]$ hostname -f
ip-172-31-37-222.us-west-2.compute.internal
[ec2-user@ip-172-31-37-222 yum.repos.d]$
[ec2-user@ip-172-31-37-222 yum.repos.d]$
[ec2-user@ip-172-31-37-222 yum.repos.d]$  df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2       40G  6.7G   34G  17% /
devtmpfs        7.3G     0  7.3G   0% /dev
tmpfs           7.2G     0  7.2G   0% /dev/shm
tmpfs           7.2G   25M  7.2G   1% /run
tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
tmpfs           1.5G     0  1.5G   0% /run/user/1000
/dev/xvdb        40G   33M   40G   1% /data
tmpfs           1.5G     0  1.5G   0% /run/user/0

[ec2-user@ip-172-31-43-23 ~]$ hostname -f
ip-172-31-43-23.us-west-2.compute.internal
[ec2-user@ip-172-31-43-23 ~]$
[ec2-user@ip-172-31-43-23 ~]$
[ec2-user@ip-172-31-43-23 ~]$  df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2       40G  1.7G   39G   5% /
devtmpfs        7.3G     0  7.3G   0% /dev
tmpfs           7.2G     0  7.2G   0% /dev/shm
tmpfs           7.2G   25M  7.2G   1% /run
tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
tmpfs           1.5G     0  1.5G   0% /run/user/1000
/dev/xvdb        40G   33M   40G   1% /data
tmpfs           1.5G     0  1.5G   0% /run/user/0

[ec2-user@ip-172-31-43-220 ~]$ hostname -f
ip-172-31-43-220.us-west-2.compute.internal
[ec2-user@ip-172-31-43-220 ~]$
[ec2-user@ip-172-31-43-220 ~]$
[ec2-user@ip-172-31-43-220 ~]$  df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2       40G  1.7G   39G   5% /
devtmpfs        7.3G     0  7.3G   0% /dev
tmpfs           7.2G     0  7.2G   0% /dev/shm
tmpfs           7.2G   25M  7.2G   1% /run
tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
tmpfs           1.5G     0  1.5G   0% /run/user/1000
/dev/xvdb        40G   33M   40G   1% /data
tmpfs           1.5G     0  1.5G   0% /run/user/0

[ec2-user@ip-172-31-34-114 ~]$ hostname -f
ip-172-31-34-114.us-west-2.compute.internal
[ec2-user@ip-172-31-34-114 ~]$
[ec2-user@ip-172-31-34-114 ~]$
[ec2-user@ip-172-31-34-114 ~]$  df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvda2       40G  1.7G   39G   5% /
devtmpfs        7.3G     0  7.3G   0% /dev
tmpfs           7.2G     0  7.2G   0% /dev/shm
tmpfs           7.2G   25M  7.2G   1% /run
tmpfs           7.2G     0  7.2G   0% /sys/fs/cgroup
tmpfs           1.5G     0  1.5G   0% /run/user/1000
/dev/xvdb        40G   33M   40G   1% /data
tmpfs           1.5G     0  1.5G   0% /run/user/0


-List the Linux release you are using
Red Hat Enterprise Linux 7.3


-List the command and output for yum repolist enabled
[ec2-user@ip-172-31-33-209 yum.repos.d]$ yum repolist enabled
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
Repo rhui-REGION-client-config-server-7 forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-client-config-server-7 forced skip_if_unavailable=True due to: /etc/pki/rhui/product/rhui-client-config-server-7.crt
Repo rhui-REGION-client-config-server-7 forced skip_if_unavailable=True due to: /etc/pki/rhui/rhui-client-config-server-7.key
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/product/content-rhel7.crt
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/content-rhel7.key
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/product/content-rhel7.crt
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/content-rhel7.key
Could not contact CDS load balancer rhui2-cds01.us-west-2.aws.ce.redhat.com, trying others.
Could not contact any CDS load balancers: rhui2-cds01.us-west-2.aws.ce.redhat.com, rhui2-cds02.us-west-2.aws.ce.redhat.com.
[ec2-user@ip-172-31-33-209 yum.repos.d]$

[ec2-user@ip-172-31-37-222 yum.repos.d]$ yum repolist enabled
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
Repo rhui-REGION-client-config-server-7 forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-client-config-server-7 forced skip_if_unavailable=True due to: /etc/pki/rhui/product/rhui-client-config-server-7.crt
Repo rhui-REGION-client-config-server-7 forced skip_if_unavailable=True due to: /etc/pki/rhui/rhui-client-config-server-7.key
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/product/content-rhel7.crt
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/content-rhel7.key
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/product/content-rhel7.crt
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/content-rhel7.key
Could not contact CDS load balancer rhui2-cds01.us-west-2.aws.ce.redhat.com, trying others.
Could not contact any CDS load balancers: rhui2-cds01.us-west-2.aws.ce.redhat.com, rhui2-cds02.us-west-2.aws.ce.redhat.com.
[ec2-user@ip-172-31-37-222 yum.repos.d]$

[ec2-user@ip-172-31-43-23 ~]$ yum repolist enabled
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
Repo rhui-REGION-client-config-server-7 forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-client-config-server-7 forced skip_if_unavailable=True due to: /etc/pki/rhui/product/rhui-client-config-server-7.crt
Repo rhui-REGION-client-config-server-7 forced skip_if_unavailable=True due to: /etc/pki/rhui/rhui-client-config-server-7.key
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/product/content-rhel7.crt
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/content-rhel7.key
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/product/content-rhel7.crt
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/content-rhel7.key
Could not contact CDS load balancer rhui2-cds01.us-west-2.aws.ce.redhat.com, trying others.
Could not contact any CDS load balancers: rhui2-cds01.us-west-2.aws.ce.redhat.com, rhui2-cds02.us-west-2.aws.ce.redhat.com.
[ec2-user@ip-172-31-43-23 ~]$

[ec2-user@ip-172-31-43-220 ~]$ yum repolist enabled
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
Repo rhui-REGION-client-config-server-7 forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-client-config-server-7 forced skip_if_unavailable=True due to: /etc/pki/rhui/product/rhui-client-config-server-7.crt
Repo rhui-REGION-client-config-server-7 forced skip_if_unavailable=True due to: /etc/pki/rhui/rhui-client-config-server-7.key
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/product/content-rhel7.crt
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/content-rhel7.key
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/product/content-rhel7.crt
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/content-rhel7.key
Could not contact CDS load balancer rhui2-cds01.us-west-2.aws.ce.redhat.com, trying others.
Could not contact any CDS load balancers: rhui2-cds01.us-west-2.aws.ce.redhat.com, rhui2-cds02.us-west-2.aws.ce.redhat.com.
[ec2-user@ip-172-31-43-220 ~]$

[ec2-user@ip-172-31-34-114 ~]$ yum repolist enabled
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos
Repo rhui-REGION-client-config-server-7 forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-client-config-server-7 forced skip_if_unavailable=True due to: /etc/pki/rhui/product/rhui-client-config-server-7.crt
Repo rhui-REGION-client-config-server-7 forced skip_if_unavailable=True due to: /etc/pki/rhui/rhui-client-config-server-7.key
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/product/content-rhel7.crt
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/content-rhel7.key
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/product/content-rhel7.crt
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/content-rhel7.key
Could not contact CDS load balancer rhui2-cds01.us-west-2.aws.ce.redhat.com, trying others.
Could not contact any CDS load balancers: rhui2-cds01.us-west-2.aws.ce.redhat.com, rhui2-cds02.us-west-2.aws.ce.redhat.com.
[ec2-user@ip-172-31-34-114 ~]$

