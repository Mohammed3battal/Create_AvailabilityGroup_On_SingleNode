## Script: Create_AvailabilityGroup_On_SingleNode.sql

**Purpose**:
Set up an Always On Availability Group on a single node (primary only) for testing, development, or pre-production setup.

**Features**:
- Starts HADR endpoint if not running
- Enables and starts AlwaysOn_health XE session
- Creates AG with no failover partners yet

**Use Case**:
- Development or QA environment with only one SQL Server instance
- Prepare AG before adding secondary replicas later

**Requirements**:
- SQL Server 2016+
- Always On Availability Groups feature enabled
- The database must be in FULL recovery mode and have a recent full backup
