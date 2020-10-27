Backup all VMs in a Cloud Service with Azure Automation
=======================================================

            

 

 This Azure Automation runbook uses Start-AzureStorageBlobCopy to copy all VHDs for all operating system and data disks for an Azure VM to a specified location.  It defaults to vhd-backups in the same storage account where
 the VHDs resides. It will shut down the operating system if the VM is running and restart it when the copy is complete - unless it is on a different storage account where the runbook will complete before the copy completes.  Runbook output logs all results.
 Use in conjunction with companion runbook Backup-AllCloudServices to backup all VMs in a subscription

 


        
    
TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group. All the Script Center fields like Rating, RatingCount and DownloadCount have been carried over to Github as-is for the migrated scripts only. Note : The Script Center fields will not be applicable for the new repositories created in Github & hence those fields will not show up for new Github repositories.
