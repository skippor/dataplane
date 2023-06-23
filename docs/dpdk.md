# 编译dpdk

## dpdk-19.11

```shell
./mk/rte.cpuflags.mk    SSE4_1
export RTE_SDK=`pwd`
./usertools/dpdk-setup.sh  38

export RTE_SDK=/mnt/dtt/dpdk/dpdk-19.11
export RTE_TARGET=x86_64-native-linuxapp-gcc
export EXTRA_CFLAGS="-O0 -g"
make config T=x86_64-native-linuxapp-gcc
make install T=x86_64-native-linuxapp-gcc
```
