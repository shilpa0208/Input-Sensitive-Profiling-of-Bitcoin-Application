# Input-Sensitive-Profiling-of-multi-threaded-Bitcoin-Application

Perfomed input-sensitive profiling on the open source multithreaded C++ application "BITCOIN". 

Bitcoin is a new worldwide digital payment system which  that enables a decentralised payment methodology  with completely digital currency. It is a peer-to-peer system in which transactions take place directly between users without an intermediary. The transactions are verified using network nodes and recorded in a public distributed ledger called blockchain. Bitcoin can be exchanged for other currencies, products and services. It can also be held as an investment. 

The open source version of this application was profiled using the **Aprof profiler** tool. 

## The problems identified were:
* Deploying the application and have it get synchroinised with the main blockchain network takes tremendous amount of time.This was the biggest challenge even before profiling it.
* Identified situtaions where the combinations of locks could significantly worsen the performance. 
* Identified lock retention and starvation which led to deadlocks which were causing performance degradation.


