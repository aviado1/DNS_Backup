# DNS Server Backup Script

This PowerShell script is designed to automate the backup process of all forward lookup zones in a DNS server environment. It simplifies the task of exporting zone configurations and copying zone files to a secure backup location.

## Features

- **Automated Backup**: Effortlessly backs up all forward lookup zones along with their configurations.
- **Export to CSV**: Zone configurations are neatly exported to a CSV file for easy management and review.
- **Customizable Backup Locations**: Users can specify backup directories for both configurations and zone files.

## Getting Started

### Prerequisites

- Windows Server with the DNS Server role installed.
- PowerShell 5.1 or higher.
- Administrative privileges on the server where the script will be executed.

### Installation

1. Clone this repository or download the script file directly.
2. Place the script in a directory of your choice on the DNS server.

### Usage

To run the script, navigate to the script's directory in a PowerShell window run as Administrator and execute:

```powershell
.\DNS_Backup_Script.ps1
