# VM Migration
VM Migration - Assess/Discover, Plan/Foundation, Migrate, Optimize

## Assess/Discover

Discover what apps a client has, using tools and interviews.

If we discover 50% with automated tools, we are lucky! Discovery is Never 100%

Migrate systems that have not been overwritten.

### Stage 1: Automated discovery**
1. Pre sales environment 
- in pre sales this discovery is for your benefit to understand what the full magnitude/scope really is.
- not for the client

2. Post sales

In the next phase (Plan and Foundation), discovery will not stop!
 
 So, in the discovery phase we are Hoping to accomplish
 - Proper quoting 
 - Time estimated for discovery (especially because this is 50% of the work in VM migration)

**Tools**
StratoZone (owned by Google now - Free)

CloudPhysics, Flexera, Cloudamize (paid-for; optinoal commercial features)

Across all tools you may still be limited at 70% discovery.

Brad also uses **Bellarc advisor** (at the server level) and do the inventory of every machine, 
Runs Advanced IP Scanner tool - IP scanners on networks, at the application level; scans applications, networking ports to figure out whats happening. 

All this is based on whether or not the client will allow you to do this). The goal is to reduce the sales cycle. Predict TCO based on various configurations for GCP. (Give yourself some wiggle room)

Spot challenges.

#### Tools collect data in three main ways
1. From vSphere or AWS - run automated discovery in a vCenter you own!!! If its multitenant you cannot do this. With that said, AWS tools are limited
2. From machines using SSH/WMI
3. From agents installed node by node
4. Data then compiled, encrypted and passed back to tool hub


CloudEndure - for bare metal migrations. AWS closed sourced it.

2016 versioned OS migration on wards (fine)

Dont consider

#### Poor first movers are:
- Highly dependent or depended upon
- Business critical and not tolerant of downtime
- Complex data environments
- Front end / Client facing apps
- Not good examples to learn and gain confidence from

### Stage 2: Survey and interviews

### Stage 3: Analysis

### Stage 4: Deliverables

In all the stages, humna intervention is required!

Be cognizant of activities that could be taking place in any service oriented application.

### Automated discovery**
