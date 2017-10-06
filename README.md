# which_zscaler
Parse information from firewalls and routers to determine Zscaler configuration

This script takes input in the form of a spreadsheet with two columns,
the first with the hostname or IP of the Cisco device, and the second
column identifying whether the device is 'cisco_ios' (for routers and
switches) or 'cisco_asa' for firewalls.

The script will log into each device, one at a time, run the commands to
obtain the desired output, parsing the key information and writing it to
another spreadsheet named "ZScaler_info_&lt;date&gt;.xlsx". This file will
automatically open when the script completes.
