# netfilter_test
Netfilter

* How2Use
gcc -o nfqnl_test nfqnl_test.c -lnetfilter_queue -Wall
sudo iptables -A OUTPUT -p tcp -j NFQUEUE
./nfqnl_test

