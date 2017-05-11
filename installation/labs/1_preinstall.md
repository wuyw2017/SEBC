### INSTALL
1. Check vm.swappiness 

root@node1 ~]# sysctl vm.swappiness
vm.swappiness = 60
[root@node1 ~]# sysctl vm.swappiness=1
vm.swappiness = 1
[root@node1 ~]# sysctl vm.swappiness
vm.swappiness = 1
[root@node1 ~]# 

2. Show the mount attributes of your volume(s)
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvde        30G  665M   28G   3% /
tmpfs           7.4G     0  7.4G   0% /dev/shm

3. If you have ext-based volumes, list the reserve space setting
[root@node1 vm]# lsblk
NAME MAJ:MIN RM SIZE RO TYPE MOUNTPOINT
xvde 202:64   0  30G  0 disk /

4. Disable transparent hugepage support
[root@node1 vm]# cat /proc/sys/vm/nr_hugepages
0

5.  List your network interface configuration
[root@node1 vm]# ifconfig -a
eth0      Link encap:Ethernet  HWaddr 06:2E:A2:E4:0D:D2  
          inet addr:172.31.36.216  Bcast:172.31.47.255  Mask:255.255.240.0
          inet6 addr: fe80::42e:a2ff:fee4:dd2/64 Scope:Link
          UP BROADCAST RUNNING MULTICAST  MTU:9001  Metric:1
          RX packets:32349 errors:0 dropped:0 overruns:0 frame:0
          TX packets:36091 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:1000 
          RX bytes:4064423 (3.8 MiB)  TX bytes:6258084 (5.9 MiB)
          Interrupt:24 

lo        Link encap:Local Loopback  
          inet addr:127.0.0.1  Mask:255.0.0.0
          inet6 addr: ::1/128 Scope:Host
          UP LOOPBACK RUNNING  MTU:16436  Metric:1
          RX packets:0 errors:0 dropped:0 overruns:0 frame:0
          TX packets:0 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:0 
          RX bytes:0 (0.0 b)  TX bytes:0 (0.0 b)

6. Show that forward and reverse host lookups are correctly resolved
[root@node1 vm]# getent hosts node1
172.31.36.216   node1

7. Show the nscd service is running   
[root@node1 vm]# service nscd status
nscd is stopped
[root@node1 vm]# service nscd start
Starting nscd: [  OK  ]
[root@node1 vm]# service nscd status
nscd (pid 13827) is running...

8. Show the ntpd service is running
[root@node1 vm]# service ntpd status
ntpd is stopped
[root@node1 vm]# service ntpd start
Starting ntpd: [  OK  ]
[root@node1 vm]# service ntpd status
ntpd (pid  13935) is running...

