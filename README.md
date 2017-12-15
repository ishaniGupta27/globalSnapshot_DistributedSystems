Global Snapshot

We all have bank accounts and do transactions everyday. When we start a transfer to another account, the money will be on the fly. It has been deducted from our account but has been not posted on the other account yet.Our application is able to take a snapshot of the global state, which means all the money in the accounts and on the fly.It is similar to checkpoints in we use in our Operating systems but more complex as we are working on distributed systems.

Getting Started

1. Run multiple client.py with unique client number(python client.py 1): This is the clients trying to take a snapshot !

config.json maintains the config details about the number of clients and ports to be used for the application.


Prerequisites

Python 2.7

Application Components:

We will assume multiple clients. Each client holds an account and have 2 oper-
ations:
1. Transfer money.
2. Start a snapshot.
Implementation:

1. Each client will start with some amount money, say 1000. We implemented the transfer function as an Automatic Transfer. We have set up money transfer of random amount every 10 seconds.
2. Each client is able to start a snapshot at anytime. A snapshot should be initialized by entering a "snap" command.


Authors

Ishani Gupta
Vivek Pradhan



Acknowledgments

Thanks to Prof. Amr El Abbadi, Computer Science Department, UCSB
