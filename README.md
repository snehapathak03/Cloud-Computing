# Cloud-Computing

<h1>DAY 1 — INTRODUCTION TO CLOUD COMPUTING</h1>
<h3>MODULE 1 — WHAT IS CLOUD COMPUTING:</h3> <p>Delivering computing services like servers, storage, databases, networking, 
and software over the internet.Instead of buying expensive computers/servers physically, companies rent resources online.<br>
<u>REAL-LIFE EXAMPLE</u>:Suppose you start a website->Without cloud:You buy server hardware,Setup networking,Handle cooling,Manage
 electricity,Repair hardware.<br>With cloud:You rent everything online instantly.That is cloud computing.
EASY EXAMPLE:Netflix uses cloud servers.Google Drive:Files stored online instead of your computer.That is cloud storage.<br>
Cloud providers give:Servers,Storage,Databases,Networking,Security,Applications,through internet.</p><br>
<h5>TOP CLOUD PROVIDERS</h5>
<p>
1. Amazon Web Services (AWS):Largest cloud provider.Used by:Netflix,NASA,Airbnb <br>
2. Microsoft Azure:Used heavily by enterprises.<br>
3. Google Cloud Platform:Strong in AI/ML.</p><br>
<pre>WHY CLOUD BECAME POPULAR->Before cloud:Companies had problems of Expensive hardware,Maintenance cost,Scaling issues,Downtime,
Space problems,Cloud solved this.</pre>
<h3>BENEFITS OF CLOUD COMPUTING</h3><p>
1. Cost Saving:No need to buy hardware.Pay only for usage.<br>
2. Scalability:Increase servers anytime.Example:Flipkart during sale,Netflix during peak traffic.<br>
3. High Availability:Cloud providers have multiple data centers.If one fails, another works.<br>
4. Global Access:Access services from anywhere.<br>
5. Fast Deployment:Servers launch within minutes.</p>

<h3>MODULE 2 — HISTORY OF CLOUD COMPUTING</h3><p>
BEFORE CLOUD Companies used:On-Premise Infrastructure.Meaning:Physical servers inside company buildings.
Problems:Expensive,Hard to maintain,Difficult scaling.<br>
VIRTUALIZATION REVOLUTION->Then virtualization came.One physical server could run:multiple virtual machines.This
 improved efficiency.<br>
BIRTH OF AWS:In 2006:Amazon Web Services launched cloud services.Main service:EC2 (virtual servers).This changed IT forever.</p>

<h3>MODULE 3 — TRADITIONAL IT VS CLOUD</h3><p>
Traditional IT->Company buys:Servers,Storage,Networking devices.Problems:Huge upfront cost,Maintenance team needed,Slow scaling.<br>
CLOUD MODEL:Cloud provider manages infrastructure.Company rents resources online. Advantages:Flexible,Cheap,Fast.</p>
<pre>COMPARISON TABLE
Traditional IT			Cloud
Buy hardware			Rent resources
High upfront cost		Pay as you use
Slow scaling			Instant scaling
Physical maintenance	Managed by provider
Limited availability	Global availability</pre>

<h3>MODULE 4 — TYPES OF CLOUD</h3><p>
1. PUBLIC CLOUD:Services available publicly through internet.Examples:AWS,Azure,GCP.Best for:startups,apps,websites.<br>
2. PRIVATE CLOUD:Cloud used only by one organization.More secure.Used by:Banks,Government organizations.<br>
3. HYBRID CLOUD:Combination of Public cloud and Private cloud.Example:Sensitive data in private cloud,Website in public cloud.</p>

<h3>MODULE 5 — CLOUD SERVICE MODELS</h3><p>
1. IaaS (Infrastructure as a Service)Provider gives:Servers,Networking,Storage.You manage:OS,Applications.Example:EC2 in AWS.<br>
2. PaaS (Platform as a Service)Provider manages:Infrastructure and OS.You only deploy code.Example:Google App Engine.<br>
3. SaaS (Software as a Service)Complete software over internet.Examples:Gmail,Zoom,Netflix.</p>
<pre>Difference Between IaaS, PaaS, SaaS

Type	User Manages		Provider Manages
IaaS	Apps, OS			Hardware
PaaS	Application			OS + Hardware
SaaS	Nothing				Everything
</pre>

<h3>MODULE 6 — DATA CENTERS</h3><p>
Cloud providers have huge data centers worldwide.Inside data centers:Servers,Cooling systems,Networking devices,Security systems.<br>

REAL-WORLD USE CASES-->Banking,Online banking apps,Fraud detection,Healthcare,Patient records,AI diagnosis,
E-commerce,Amazon,Flipkart,Entertainment,Netflix,Spotify.</p>

<p>WHat is the differences between aws,azure, google cloud ?<br>
What is cloud computing?<br>
Why companies use cloud?<br>
What is scalability?<br>
Difference between traditional IT and cloud.<br>
Draw architecture diagram:User → Internet → Cloud Provider → Servers → Database<br>
Create accounts:AWS Free Tier,GitHub<br>
YOUTUBE:1.AWS Cloud Computing Full Course - freeCodeCamp.2.Cloud Computing Explained - TechWorld with Nana<br>
MINI QUIZ<br>
Q1.Which cloud model gives complete software online?->SaaS<br>
Q2.Which company launched AWS?->Amazon<br>
Q3.Which service model gives virtual machines?->IaaS
</p>

<h1> DAY 2 — VIRTUALIZATION, VMs & CONTAINERS</h1>
<h3>MODULE 1 — WHAT IS VIRTUALIZATION</h3><p>
THE MAIN PROBLEM BEFORE VIRTUALIZATION WAS:Earlier:One company bought:1 physical server.But used:only 10–20% power.<br>
Remaining resources were wasted.Example:A server may have:64 GB RAM and  16 CPU cores.But application only uses:
8 GB RAM and 2 CPU cores.Huge wasteage.SOLUTION = VIRTUALIZATION-->Virtualization allows:One physical computer 
to run multiple virtual computers.These virtual computers are called:Virtual Machines (VMs).<br>
REAL-WORLD EXAMPLE:Think of a big apartment building.Physical Server = Building and Virtual Machines = Different apartments
Each apartment:separate,isolated,independent. But all share same building.</p>
<p>HOW VIRTUALIZATION WORKS:A special software layer creates virtual machines.That software is called:Hypervisor.</p>

<h3>MODULE 2 — HYPERVISOR</h3><p>
WHAT IS A HYPERVISOR?A hypervisor is software that:creates VMs,manages VMs,allocates hardware resources.<br>
It sits between:Hardware and Virtual Machines.<br>
ARCHITECTURE:Application → Virtual Machine → Hypervisor → Physical Hardware<br>
<u>TYPES OF HYPERVISORS</u><p>
TYPE 1 HYPERVISOR (Bare Metal):Runs directly on hardware.Very fast and secure.Examples:VMware ESXi,Microsoft Hyper-V,KVM.
Used in:AWS,Azure,Google Cloud<br>
TYPE 2 HYPERVISOR:Runs on top of operating system.Examples:Oracle VM VirtualBox and VMware Workstation.Mostly used 
for:learning and testing.</p></p>
<pre>DIFFERENCE
Type 1					Type 2
Directly on hardware	On operating system
Faster					Slower
Enterprise use			Personal use
More secure				Less secure
</pre>

<h3>MODULE 3 — VIRTUAL MACHINES (VMs):</h3><p>
A VM is a software-based computer.It behaves like real computer.VM has:OS,CPU,RAM,Storage and Applications.
Each VM has:separate operating system and separate resources.Example:One server can run:Ubuntu VM,Windows VM,Kali Linux VM,
all together.</p>
<p>WHY CLOUD USES VMs-->Cloud providers use virtualization because:Better hardware utilization, Isolation, Scalability, 
Easy management, Fast deployment.AWS EXAMPLE:When you launch:Amazon EC2->you are basically launching:a virtual machine.</p>
<h6>VM ADVANTAGES</h6><p>
1. Isolation->If one VM crashes:others still work.<br>
2. Better Resource Usage->Multiple VMs use same server.<br>
3. Flexibility->Different operating systems possible.</p>
<h6>VM DISADVANTAGES</h6><p>
1. Heavy->Each VM has full operating system.Consumes:RAM,storage,CPU.<br>
2. Slow Boot->VM startup takes time.</p>

<h3>MODULE 4 — INTRODUCTION TO CONTAINERS</h3><p>
WHAT IS A CONTAINER?A container is a lightweight package containing application + dependencies.It shares host operating system.<br>
MAIN DIFFERENCE<br>
VM:includes full OS and Container:shares host OS kernel.Therefore containers are:smaller,faster and lightweight.<br>
REAL-WORLD EXAMPLE:Imagine:VM = Full separate house and Container = Separate room inside same house.<br>
WHY CONTAINERS BECAME POPULAR:Developers had problem:Application works on my laptop,but not on server. Containers solved this.<br>
CONTAINER ADVANTAGES: Fast startup, Lightweight, Portable, Consistent environments, Better scalability.<br>
MOST POPULAR CONTAINER TOOL->Docker</p>

<h3>MODULE 5 — VM VS CONTAINER</h3><pre>
Virtual Machine			Container
Full OS included		Shares OS
Heavy					Lightweight
Slow startup			Fast startup
More resource usage		Less resource usage
Better isolation		Less isolation
GBs in size				MBs in size</pre>

<h3>MODULE 6 — HOW CLOUD USES THESE TECHNOLOGIES</h3><p>
Cloud providers combine:Virtualization,Containers,Networking,Automation,to provide services instantly.Example:When AWS 
launches EC2:hypervisors create virtual machines.When Kubernetes runs applications:containers are used.</p>

<pre>TASK 1 — INSTALL VIRTUALBOX->Install:Oracle VM VirtualBox Official Website
TASK 2 — INSTALL UBUNTU ISO->Download Ubuntu ISO:Ubuntu Desktop Download
TASK 3 — CREATE YOUR FIRST VM->Inside VirtualBox:Create:Ubuntu VM. Give:4 GB RAM,2 CPU cores,25 GB storage
TASK 4 — EXPLORE UBUNTU:Learn:terminal,settings,file system
BASIC LINUX COMMANDS TO TRY->pwd,ls,cd,mkdir test,rm -r test
TASK 5 — SYSTEM INFO COMMANDS:uname -a,free -h,df -h,top
Cloud engineers spend huge time in Linux terminal.Become comfortable with command line early.
YOUTUBE VIDEOS FOR TODAY
1 — Virtualization Explained->Virtualization Explained - TechWorld with Nana
2 — Containers vs VMs->Containers vs Virtual Machines - IBM Technology
3 — Ubuntu Installation->Install Ubuntu on VirtualBox
MINI QUIZ
Q1.Which software creates virtual machines?->Hypervisor
Q2.Which is lighter:VM or Container?->Container
Q3.Which AWS service gives virtual machines?->Amazon EC2
 How cloud providers run thousands of servers
 What virtualization actually means
 Why containers changed DevOps completely</pre>