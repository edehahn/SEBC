'''[root@ip-172-31-18-209 ~]# cat /proc/sys/vm/swappiness
1
[root@ip-172-31-18-209 ~]# grep swap /etc/sysctl.conf
vm.swappiness = 1'''

'''LABEL=_         /                       ext4    defaults        1 1
tmpfs                   /dev/shm                tmpfs   defaults        0 0
devpts                  /dev/pts                devpts  gid=5,mode=620  0 0
sysfs                   /sys                    sysfs   defaults        0 0
proc                    /proc                   proc    defaults        0 0'''

'''[root@ip-172-31-18-209 ~]# tune2fs -l /dev/xvde1
tune2fs 1.41.12 (17-May-2010)
Filesystem volume name:   _
Last mounted on:          /
Filesystem UUID:          dcb1645e-05a6-4311-8bce-a9c12bec5801
Filesystem magic number:  0xEF53
Filesystem revision #:    1 (dynamic)
Filesystem features:      has_journal ext_attr resize_inode dir_index filetype needs_recovery extent flex_bg sparse_super large_file huge_fil                                e uninit_bg dir_nlink extra_isize
Filesystem flags:         signed_directory_hash
Default mount options:    user_xattr acl
Filesystem state:         clean
Errors behavior:          Continue
Filesystem OS type:       Linux
Inode count:              524288
Block count:              2096896
Reserved block count:     104844
Free blocks:              1777687
Free inodes:              503620
First block:              0
Block size:               4096
Fragment size:            4096
Reserved GDT blocks:      511
Blocks per group:         32768
Fragments per group:      32768
Inodes per group:         8192
Inode blocks per group:   512
Flex block group size:    16
Filesystem created:       Mon Sep 29 22:17:58 2014
Last mount time:          Mon Jun  5 14:17:39 2017
Last write time:          Thu Oct  2 17:03:03 2014
Mount count:              7
Maximum mount count:      -1
Last checked:             Mon Sep 29 22:17:58 2014
Check interval:           0 (<none>)
Lifetime writes:          1909 MB
Reserved blocks uid:      0 (user root)
Reserved blocks gid:      0 (group root)
First inode:              11
Inode size:               256
Required extra isize:     28
Desired extra isize:      28
Journal inode:            8
Default directory hash:   half_md4
Directory Hash Seed:      7039363b-3a6a-46d3-bc61-7dd2a90f3a4b
Journal backup:           inode blocks'''
