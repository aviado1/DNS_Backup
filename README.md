# DNS Forward Lookup Zone Backup Script

This PowerShell script provides an automated approach to back up all forward lookup zones on a DNS server, targeting environments where the DNS server role is installed on Windows Server. It facilitates the export of zone configurations to a CSV file and backs up the actual zone files to a designated directory.

## How It Works

The script performs several key operations:

1. **Defines the Backup Directory:** It sets a base directory for the backups and a child directory for the zone files. It also defines a path for the configuration export file, incorporating the current date for versioning.
2. **Checks for Directory Existence:** Before proceeding with the backups, it ensures that the specified directories exist, creating them if necessary.
3. **Exports Zone Configurations:** It filters for primary forward lookup zones that are not reverse lookup zones and exports their configurations to the predefined CSV file path.
4. **Backs Up Zone Files:** For each eligible zone, it locates the zone file and copies it to the backup directory, ensuring that both configuration data and zone data are preserved.

## Prerequisites

Before running this script, ensure that:
- You have administrative access to the DNS server.
- PowerShell is enabled and can execute scripts (adjust your execution policy if necessary).

## Usage

To use this script:

1. Modify the `$backupBaseDir` variable at the beginning of the script to specify your backup directory.
2. Run the script in a PowerShell terminal with administrative privileges.

## Script Author

This script was authored by [aviado1](https://github.com/aviado1), dedicated to enhancing system administration practices through efficient scripting.

## Disclaimer

This script is provided "as is," with no guarantees. Always test scripts in a safe, non-production environment before deployment.

## Contributions

Your contributions are welcome! If you have suggestions for improvement or have identified bugs, please fork the repository, make your changes, and submit a pull request.

