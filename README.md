# netfilter_test
Netfilter

* Environment

Ubuntu 16.04.02 LTS

* Dependency
```sh
sudo apt-get install libnetfilter-queue-dev
```

* How2Use

Using two terminals

Terminal-1
```sh
zanywhale@ubuntu:$ gcc -o nfqnl_test nfqnl_test.c -lnetfilter_queue -Wall
zanywhale@ubuntu:$ sudo ./nfqnl_test
```

Terminal-2
```sh
zanywhale@ubuntu:$ sudo iptables -A OUTPUT -p tcp -j NFQUEUE
zanywhale@ubuntu:$ sudo iptables -F
```

