###Overview
Using the latest available image for Windows Server 2012 R2 in the azure gallery, it will create a Windows Failover Cluster with quorum configuration 'Node and File Share Majority'. Active directory infrastructure should already have been deployed.

###Virtual Machines (VMs)
1.The number of cluster VMs is controlled by the input parameter 'NumberOfClusterNodes, but a minimum of two is needed for creating a valid cluster.
2.A single VM for having a 'Node and File Share Majority' quorum configuration in the failover cluster, with the VM acting as a 'file share witness'.

###Limitations
Following are the limitations of this template. Users can fork this repository and customize the template to fix them or wait for our periodic updates.
> - The template does not allow specifying the quorum configuration. However, it uses ''Node and File Share Majority' which is optimal for deployment on Windows Azure.

###References
Please refer to the following links for more information on SQL Server Availability Groups.
> - [Windows Failover Cluster](http://technet.microsoft.com/en-in/library/hh831579.aspx)