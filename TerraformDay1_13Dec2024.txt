#I will record each and everything I have learned during my Terraform training in this note. This will be quick reference.

Infrastructure as a code:

A story: 

Phani was tasked with building a Kubernetes cluster that contains 3 control plane nodes and 10 worker nodes and the deadline to deliver them is 2 days. Now, Phani is thinking how can I provid infra and configure kubernetes cluster on them in such a short notice.Normally, when Phani has started his career, this type of provisioning the infra requires identifying the prerequisites,coordinating with different teams like OS,Network,Storage,Application,Database,Middleware etc and then manually building each and every server as per the plan charted. The configuration for all the three control plane nodes should be identical and the config for the 10 worker nodes should be identical. So, he started working on the same and for each server it took 2 hours and total estimated time is 26 hours(excluding the time for the OS team to build the servers ~ 13) to configure the infrastructure. For each server he is making the notes and utilizing the same notes for other servers. The problem here is He might make a mistake while taking notes, this notes is on his local machine and other team members cannot see or utilize it, he is building and configuring each and every server manually and repeating the same process for all the servers.This is tedious process and will take lot of time.

The moral : Work smart but not hard

What if I tell you there is a solution for it? 
And what if I tell you that you can build the same infrastructure in a matter of minutes -forget about hours ?
And will you be surprised that you only need to pass the information in a code which is very simplified language where you define the infrastructure and other dependencies ?

Yes, you heard it right. This is called as Infrastructure as a code.


There are several players that are providing this IAC.

	> Terraform
	> Pulumi
	> AWS Cloud Formation
	> Azure Resource Manager
	> Openstack Heat
	> GCP related IAC

Out of all the above Terraform can show its true power on all the cloud platforms and is the King.
