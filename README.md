# oracle-database-ansible-samples

Different database tasks automated using Ansible.

---

**DISCLAIMER:**  
THE CONTRIBUTIONS IN THIS ORGANIZATION WERE NOT REVIEWED BY ORACLE EMPLOYEES. THE REPOSITORIES WERE ALSO NOT REVIEWED FOR SECURITY CONCERNS. USE AT YOUR OWN RISK.

## Installation

This repository contains Ansible playbooks for Oracle Database 21c setup and management. Below are the requirements for installation:

- OS: OEL 7.5
- Ansible Version: 2.7.6
- Database Version: Oracle 21.3 Linux64

**Setup Instructions:**
1. Download the required Oracle software from [Oracle Technology Network (OTN)](http://www.oracle.com/technetwork/indexes/downloads/index.html) or My Oracle Support (MOS), depending on your support status.
2. Stage the Oracle binaries from "edelivery: Oracle Database 21c Software (64-bit)".
3. Follow the tasks outlined in each role for your desired configuration.

## Documentation

Refer to Oracle's official documentation for detailed installation and upgrade guides:

- [Grid Infrastructure Installation and Upgrade Guide for Linux](https://docs.oracle.com/en/database/oracle/oracle-database/21/install-and-upgrade.html)
- [Database Installation Guide for Linux](https://docs.oracle.com/en/database/oracle/oracle-database/21/ladbi/index.html)

## Examples

This repository includes roles for specific Oracle Database tasks. Below is a summary of the roles and their functionality:

| Role                   | Description                                                                                                                                          |
|------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------|
| dbsoftware21c_install | Install Oracle SI database software on multiple servers. [View role](https://github.com/asiandevs/oracle21c/tree/main/roles/dbsoftware21c_install)   |
| cdb_create_21c        | Deploy an empty Container Database (CDB). [View role](https://github.com/asiandevs/oracle21c/tree/main/roles/cdb_create_21c)                        |
| pdb21c_create         | Deploy a pluggable database (PDB) to an existing CDB. [View role](https://github.com/asiandevs/oracle21c/tree/main/roles/pdb21c_create)             |
| sbdb21c_create        | Create a physical standby database and set up Data Guard Broker. [View role](https://github.com/asiandevs/oracle21c/tree/main/roles/sbdb21c_create) |
| racgi21c_install      | Install Oracle Grid Infrastructure. [View role](https://github.com/asiandevs/oracle21c/tree/main/roles/racgi21c_install)                            |
| racdbsoft21c_install  | Install Oracle RAC software. [View role](https://github.com/asiandevs/oracle21c/tree/main/roles/racdbsoft21c_install)                                |
| racdb21c_create       | Create a two-node RAC database. [View role](https://github.com/asiandevs/oracle21c/tree/main/roles/racdb21c_create)                                  |
| racdb21c_patch_apply  | Apply GI and database release updates for 21c (October 2021). [View role](https://github.com/asiandevs/oracle21c/tree/main/roles/racdb21c_patch_apply) |
| racgi_ss_21c_install  | Configure Oracle Grid Infrastructure for a standalone server. [View role](https://github.com/asiandevs/oracle21c/tree/main/roles/racgi_ss_21c_install) |
| oracleclient21c_install | Deploy Oracle Database 21c Client for Linux x86–64. [View role](https://github.com/asiandevs/oracle21c/tree/main/roles/oracleclient21c_install)   |

## Help

For questions related to these playbooks, feel free to contact me or open an issue in this repository.

---

**NOTE:**  
Please modify these playbooks based on your own setup. This is purely based on a personal lab setup.
