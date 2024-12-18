# tc-kuka-agilus

TwinCAT code for the KUKA Agilus R700-2 Robot at Campus Verftet. Mainly safety config using FSoE (Fail Safe over EtherCAT).

There is a known issue where links between aut and safety get dropped. Basically the HMI don't work. One solution is to recreate the safety project, should be improved. See https://github.com/frdedynamics/tc-kuka-agilus/issues/1

## Getting Started

Pre flight checks

1. Check cabling including cable to your laptop from IPC

Startup

1. Power on KUKA Agilus R700-2.
1. Power on Beckhoff IPC
1. Open TwinCAT..
1. Activate configuration, Yes to run
1. Open Visualization, log in, yes if prompted for download
1. Click Run/Stop to on
1. Click Reset to reset the E-stop from cold start.

Download safety project

1. Go to SAFETY, Target System, copy serial number of safety controller EL6910 to clipboard
1. Open TwinSafeGroup.sal
1. Download safety Project. User Administrator, serial number from clipboard, default pw TwinSAFE
1. Select Complete Project Data
