# VMotion_IT13110680
##Description on VMotion

VMotion empowers the live relocation of running virtual machines starting with one physical server then onto the next with zero downtime, constant administration accessibility, and complete exchange honesty. It is straightforward to clients.

VMotion enables,
  •	Automatically upgrade and distribute whole pools of assets for most extreme equipment usage and accessibility. </n>
  •	Perform equipment support with no planned downtime. 
  •	Proactively relocate virtual machines far from falling flat or failing to meet expectations servers.
Working procedure of VMotion
In the first place, the whole condition of a virtual machine is typified by an arrangement of documents put away on shared stockpiling. VMware's bunched Virtual Machine File System (VMFS) permits numerous establishments of ESXI Server to get to the same virtual machine documents simultaneously. 
Second, the dynamic memory and exact execution condition of the virtual machine is quickly exchanged over a fast system. This permits the virtual machine to promptly change from running on the source ESXI Server to the goal ESXI Server. VMotion keeps the exchange time frame vague to clients by monitoring on-going memory exchanges in a bitmap. Once the whole memory and framework state has been duplicated over to the objective ESXI Server, VMotion suspends the source virtual machine, duplicates the bitmap to the objective ESXI Server, and resumes the virtual machine on the objective ESXI Server. This whole procedure takes under two seconds on a Gigabit Ethernet system. 
Third, the systems utilized by the virtual machine are additionally virtualized by the hidden ESXI Server. This guarantees even after the relocation, the virtual machine system character and system associations are protected. VMotion deals with the virtual MAC address as a major aspect of the procedure. Once the goal machine is actuated, VMotion pings the system switch to guarantee that it knows about the new physical area of the virtual MAC address. Since the movement of a virtual machine with VMotion safeguards the exact execution express, the system personality, and the dynamic system associations, the outcome is zero downtime and no disturbance to clients.

Requirements for VMotion
  •	The hosts must be running EXSi 5.1 or later.
  •	The host must be licensed for VMotion.
  •	The hosts must meet the networking requirement for VMotion.
  •	The virtual machines must be properly configured for VMotion.
  •	Virtual machine disks must be in persistent mode or be raw device mappings (RDMs)
  •	The destination host must have access to the destination storage.
  •	When you move a virtual machine with RDMs and do not convert those RDMs to VMDKs, the destination host must have access to the RDM LUNs.
  •	Consider the limits for simultaneous migrations when you perform a VMotion migration without shared storage. This type of VMotion counts against the limits for both VMotion and Storage VMotion, so it consumes both a network resource and 16 data store resources. 
  
  Step 1: Go to configuration and click on Networking.

