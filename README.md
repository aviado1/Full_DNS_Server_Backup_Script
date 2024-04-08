# Full DNS Server Backup Script

This PowerShell script provides a comprehensive solution for backing up the entire DNS server, including all forward lookup zones and server-wide settings. It's designed to ensure that DNS server configurations and zone files are safely archived, which can be crucial for disaster recovery and server migration scenarios.

## Features

- **Comprehensive Backup**: Backs up DNS server settings, forward lookup zone configurations, and zone files.
- **Customizable Backup Location**: Allows specifying the backup directory for storing configuration exports and zone files.
- **Export Formats**: Exports DNS configurations to CSV and XML files for easy review and documentation.

## Prerequisites

To run this script, you will need:
- PowerShell 5.1 or higher.
- DNS Server role installed on the machine where the script will be executed.
- Administrative privileges to access and modify DNS settings and to create backup directories.

## Usage

1. **Download the Script**: Download the `Full_DNS_Server_Backup_Script_AviadOfek.ps1` from this repository.
2. **Customize the Script (Optional)**: Modify the `$backupBaseDir` variable within the script to change the default location where backups are stored.
3. **Execute the Script**: Run the script in a PowerShell session with administrative privileges. The script will create the necessary directories, export the DNS server settings, and copy the zone files to the specified backup location.

### Running the Script

To run the script, open PowerShell as an Administrator and navigate to the directory containing the script. Execute the script by typing:

```powershell
.\Full_DNS_Server_Backup_Script_AviadOfek.ps1
