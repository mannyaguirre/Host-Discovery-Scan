# Implementing a Tenable Host Discovery Scan: Cyber Range

<img width="703" height="342" alt="TenableCyberRange" src="https://github.com/user-attachments/assets/40ae31ab-0d60-4601-95e8-df67b2a6ce39" />

## Overview

In this lab I did a Host Discovery Scan for Log(N) Pacific's Cyber Range environment. I used a Host Discovery Scan template on Tenable Vulnerability Management, chose the designated IP range from Log(N) Pacific's Cyber Range in Microsoft Azure, reviewed the results of the scan, properly labeled the devices found in the network.

---

## Lab Objectives

By the end of this lab I was able to:

- Create a Host Discovery Scan on Tenable
- Find the target IP address range on Microsoft Azure
- Review the results of the unkown assets
- Tag the assets based on ownership, asset type and criticality

---

## Tools Used

- Tenable Vulnerability Management
- Microsoft Azure
- Nessus Scanner: Host Discovery

---

## Lab Enviroment

| Component | Description |
|---|---|
| Scanner Type | Nessus Scanner |
| Scan Type | Host Discovery  |
| Platform | Tenable Vulnerability Management |
| Platform | Microsoft Azure |
| IP Address Target | 10.0.0.0/21 |

---

## Lab Steps

### Step 1

The first step was to select the ***Host Discovery Scan*** template in Tenable. The target IP ranger was ```10.0.0.0/21``` which was found in Microsoft Azure as shown in ***Exhibit 3***. In a typical enterprise enviroment you would get in communication with the network team or IT team and ask for the private IP range of the company so you can run the Host Discovery Scan. The scan started after the template was selected along with the target IP range.

### Why This Matters?

In a regular enterprise enviroment it is common to run Host Discovery scans monthly to make sure  all the assets connected to the company's network are accounted for and properly documented based on the company's needs. For example, asset onwership, the criticaility of the asset, the type of assest etc. 


### Exhibit 1
<img width="1918" height="978" alt="lab1" src="https://github.com/user-attachments/assets/4e34a9f4-662a-45f6-a71c-1ee7e3233244" />

### Exhibit 2
<img width="1918" height="980" alt="Lab3" src="https://github.com/user-attachments/assets/97d38c27-9ac7-410b-afe0-8967cf78e24a" />

### Exhibit 3
<img width="1917" height="941" alt="Lab2" src="https://github.com/user-attachments/assets/438b05c8-5335-44cb-bd2e-3c623ec4c378" />

---

### Step 2

The second step was to review the results of the Host Discovery Scan and obverse assets unknown to the network. Note that the scan did not yield any results for vulnerabilities as shown in the blue box in ***Exhibit 4*** because the ***Host Discovery scan only finds assets***. There are other types of scans such as a Nessus Agent Scan that find vulnerabilities. The results yield four assets found and a total of 2,048 IP addresses scanned. The scan was completed in approxiamtely 11 minutes.  

### Why This Matters?

It is important to review the assets found in the Host Discovery scan to make sure the assets are properly labeled inside of the network and not have any rogue devices within the network. In addition, it is important to account for the assets within the network to spot any possible malicous rogue devices connected by a threat actor. 

### Exhibit 4
<img width="1918" height="978" alt="Lab4" src="https://github.com/user-attachments/assets/3fb31ccb-5778-4afa-a2b7-7fb8c36ad66e" />

### Exhibit 5
<img width="1918" height="980" alt="Lab5" src="https://github.com/user-attachments/assets/6b2f1de4-2b40-43af-9934-2b5f59c069b2" />

---

### Step 3

The third step was to properly label the assets found by the scan. This is done directly on Tenable as shown in ***Exhibit 5 and Exhibit 6***. Tenable offers a prebuilt list of categories for assets along with a customizable option. 


### Why This Matters?

It is important to label all the assets found by the scan because it helps protect company assets, helps an organization be complaint during an audit, it helps with asset management.

   
### Exhibit 5
<img width="1918" height="977" alt="Lab5 9" src="https://github.com/user-attachments/assets/94dfae6c-d34a-44c7-93e5-a02f9f5a9fbd" />

### Exhibit 6
<img width="1918" height="982" alt="Lab6" src="https://github.com/user-attachments/assets/b14bc108-99b1-40f6-a063-fb4a61c1cdbb" />

---

### Rogue device not recognized, what do you do? P.O.A.M

 Any rogue devices not recognized could be harmful to the company's network. In the case that a rogue device is found and no ownership can be verified you can take the following steps:

1. **Isolate the device** - Disconnect the rogue device from the network to prevent any unautharized access.
2. **Investigate** - Analyze the rogue device to understand its purpose and security status using security tools.
3. **Decide** - Follow your organization's security policies to either remove, secure or reingrate the device to the network.


## Key Takeaways

- Host Discovery Scans only find assets and not vulnerabilities.
- Monthly Host Discovery scans is a common practice with companies.
- Properly label any assets found by the Host Discovery Scan.
- Any rogue devices must be isolated, investigated and be removed or reintegrated based on company's security policies.

---

## Conclusion

In this lab I succesfuly created  a Host Discovery scan using Tenable Vulnerability Management. I scanned an IP range of Log(N) Pacific's Cyber Range of 2,048 IP addresses. The results yield four unknow assets on the network. The asset were labeled according to ownership, criticality and device type. 

This lab help me enforce my understanding Host Discovery Scan, labeling found assets and plan of action for unknowm rogue devices. 

---

```
Author        : Manuel Aguirre
LinkedIn      : linkedin.com/in/mannyaguirre/
GitHub        : github.com/mannyaguirre
Date Created  : May 7, 2026
Last Modified : May 7, 2026
Version       : 1.0
```

