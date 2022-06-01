Fork: [https://github.com/yoshinorim/mha4mysql-manager](https://github.com/yoshinorim/mha4mysql-manager)

See https://github.com/yoshinorim/mha4mysql-manager/wiki for details.

### Note

由于原项目已经有4年无人维护，在我司产品中使用过程中发现了一些问题，所以fork一份自行修改。

### Installation

```shell
yum -y install perl-DBD-MySQL perl-Module-Install

tar -xvf mha4mysql-manager-0.58.tar.gz

# 执行后会创建真正的 Makefile
perl Makefile.PL

# 执行安装
make && make install 

# 看到如下组件则证明mha-master组件安装完毕
[root@localhost mha4mysql-manager-0.58]# ll /usr/local/bin/
总用量 184
-r-xr-xr-x  1 root root 17639 6月   1 15:33 apply_diff_relay_logs
-rwxr-xr-x. 1 root root 95104 3月  12 2021 blur_image
-r-xr-xr-x  1 root root  4807 6月   1 15:33 filter_mysqlbinlog
-r-xr-xr-x  1 root root  1995 6月   1 15:49 masterha_check_repl
-r-xr-xr-x  1 root root  1779 6月   1 15:49 masterha_check_ssh
-r-xr-xr-x  1 root root  1865 6月   1 15:49 masterha_check_status
-r-xr-xr-x  1 root root  3201 6月   1 15:49 masterha_conf_host
-r-xr-xr-x  1 root root  2517 6月   1 15:49 masterha_manager
-r-xr-xr-x  1 root root  2165 6月   1 15:49 masterha_master_monitor
-r-xr-xr-x  1 root root  2373 6月   1 15:49 masterha_master_switch
-r-xr-xr-x  1 root root  5172 6月   1 15:49 masterha_secondary_check
-r-xr-xr-x  1 root root  1739 6月   1 15:49 masterha_stop
-r-xr-xr-x  1 root root  8337 6月   1 15:33 purge_relay_logs
-r-xr-xr-x  1 root root  7525 6月   1 15:33 save_binary_logs
```
