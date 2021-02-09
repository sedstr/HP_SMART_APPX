# HP_SMART_APPX
appX version of HP Smart tool version 115.1.152.0 without the email registration requirment.

The app will still attempt to automatically update itself and does not provide a 'dont update' option.
A firewall rule is required, to prevent the HP.Smart.exe from accessing the Internet.

Click the 'open printer app' link under the printer in windows 'Printers and Scanners'
Dont click 'update', simply leave it on screen for the moment
Open up task manager, go to the details tab and find the 'HP.Smart.exe' process
rclick on the process and open file location
select in the address field and copy the path
Open 'Windows Defender Firewall with Advanced Security'
Select 'outbound rule' on the left, then 'new rule' on the right
Select 'program' as the rule type and click next
Select 'This program path:' and paste the path copied from the proces file location explorer window, then click browse
Select HP.Smart.exe and click open, then next
Block a connection, next
Tick all boxes, Domain, Private, Public and next
Give it a name that you can find in the firewall list
Find the rule, rclick - properties
Select the scope tab, then under Remote IP address, select 'These IP addresses' and click add (Local IP address leave as any)
Select 'Internet' from 'Predefined set of computers' dropdown
Apply and OK
Now if you still have the HP Smart window open, with 'update', hit the X on the window
Check task manager, to confirm HP.Smart.exe is not listed, then click the 'open printer app'... should let you straight in.
Seems like a long list of steps, but its not that hard.




