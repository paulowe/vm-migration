# Stratozone
Use StratoZone to get a detailed view of the VMs in the datacenter, what's running on them, and how they are interacting. In addition, you will configure StratoZone's settings for generating rightsize recommendations for the GCE environment.

**Tasks**
### 1. Generate VM inventory details and an overview of what is running where (Analyze vSphere)
StratoZone breaks it's analysis into three major modules. Analyze provides information about the current environment, and it will work with vSphere, AWS, Azure, GCP, bare metal, etc. 

Plan then allows the user to plan details of an upcoming migration. 

Migrate, which isn't currently included with the free-to-partners Google-StratoZone deal, has some actual migration features

**Analyze module** is broken down into
- Dashboard
![Screen Shot 2021-07-26 at 3 30 33 PM](https://user-images.githubusercontent.com/40435982/127047453-bcb6961c-dba6-4c44-b448-18d6416a9efb.png)

- Summary
- Assessments - Assessments would typically be the starting point in a new data collection. From this tab, the user can create, monitor, and manage data collectors (StratoProbes). Adding a new assessment (+ button next to Manage Assessments) would send a link to an email address of your choice, and the recipient would download and install the StratoProbe in their respective data center. The StratoProbe would be given network and credential access to the VMs, to the StratoZone mother ship (hosted in GCP), to vCenter, and SSH/WMI access to the VMs.
- Inventory - The StratoProbe uses SSH/WMI to access the VM, it then probes for details related to resources, installed software, machine name, location, IP, CPU, storage, and memory, all of which are pulled into the details tab, along with a guess as to the machine role and likely org unit.
- Dependency
- StratoFit
- Utilization
- Reports

[Guide for running the StratoProbe Data Collector(s)](https://docs.google.com/presentation/d/1iNS2BXelxUgBbtmIQyOa3WhS79Eh17CWOMU_UzTrkdA/present?slide=id.gc7d8d4bb0b_7_425)


2. Set defaults for the GCE machine mappings and TCO estimations

When StratoZone investigates machines with SSH/WMI, it uses netstat to analyze how those machine are communicating with machines over the network. Over time, it builds up a map of inter-machine communication.


3. Use StratoZone's Dependency+ feature to generate an automated view of machine dependencies

