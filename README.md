# Homework
Setup and configure virtual machine
## 1. Homework 1
### 1. Setup virtual machine
* Window server 2k8 ( host only mode )
  * 2 GB Ram
  * 50 GB storage
    * C 40 GB ( name: Window 2k8 )
    * D 10 GB ( name: DATA )
* Window 2007 ( host only mode )
### 2. Netowrk and naming
* Window server :
  * Network
    * Subnet: 192.168.1x.250
    * SubnetMask: 255.255.255.0
    * DefaultGateway: 192.168.1x.1
    * DNSServer: 192.168.1x.250
  * Name
    * HQDSERVER
### 3. DCPROMO
* mame: hqd.edu.vn
* password: @dmin123
### 4. Group Policy
`Window` > `Group policy management` > `hqd.edu.vn` > `edit`
* Turn off password complexity policy
* Lockout policy: 2
* Turn off Task manager
Open cmd with `administrator` and run:
```
gpupdate
```
### 5. Add user
Open cmd with `administrator` and run:
```
net user hv1 /add
net user hv2 /add
net user hv3 /add

net user tn1 /add
net user tn2 /add
net user tn3 /add
```

`Window active` > Add group
* HOC_VIEN
* TOT_NGHIEP

### 6. Add folder
### 7. Map drive
### 8. Add printer
