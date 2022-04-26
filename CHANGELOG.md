o Changelog :
    [x] Version 5.4cr - 26/04/2022
        * Added -dfir option which runs DFIR specific modules/collection
        * Added AllBoxes function to capture all devices on the domain, only runs as part of -dfir option
    [ ] Version 5.3 - 03/07/2022
        * Added SamAccountName to Get-PrivilegedGroupMembership output
        * Swapped some write-host to write-both so it's captured in the consolelog.txt
    [ ] Version 5.2 - 01/28/2022
        * Enhanced Get-LAPSStatus
        * Added news checks (AD services + Windows Update + NTP source + Computer container + RODC + Locked accounts + Password Quality)
        * Added support for WS 2022
        * Fix OS version difference check for WS 2008
        * Fix Write-Progress not disappearing when done
    [ ] Version 5.1
        * Added check for newly created users and groups
        * Added check for replication mechanism
        * Added check for Recycle Bin
        * Fix ProtectedUsers for WS 2008
    [ ] Version 5.0
        * Make the script compatible with other language than English
        * Fix the cpassword search in GPO
        * Fix Get-ACL bad syntax error
        * Fix Get-DNSZoneInsecure for WS 2008
    [ ] Version 4.9
        * Bug fix in checking password comlexity
    [ ] Version 4.8
        * Added checks for vista, win7 and 2008 old operating systems
        * Added insecure DNS zone checks
    [ ] Version 4.7
        * Added powershel-v2 suport and fixed array issue
    [ ] Version 4.6
        * Fixed potential division by zero
    [ ] Version 4.5
        * PR to resolve count issue when count = 1
    [ ] Version 4.4
        * Reinstated nessus fix and put output in a list for findings
        * Changed Get-AdminSDHolders with Get-PrivilegedGroupAccounts
    [ ] Version 4.3
        * Temp fix with nessus output
    [ ] Version 4.2
        * Bug fix on cpassword count
    [ ] Version 4.1
        * Loads of fixes
        * Works with Powershellv2 again now
        * Filtered out disabled accounts
        * Improved domain trusts checking
        * OUperms improvements and filtering
        * Check for w2k
        * Fixed typos/spelling and various other fixes
    [ ] Version 4.0
        * Added XML output for import to CheckSecCanopy
    [ ] Version 3.5
        * Added KB more references for internal use
    [ ] Version 3.4
        * Added KB references for internal use
    [ ] Version 3.3
        * Added a greater level of accuracy to Inactive Accounts (thanks exceedio)
    [ ] Version 3.2
        * Added search for DCs not owned by Domain Admins group
    [ ] Version 3.1
        * Added progress to functions that have count
        * Added check for transitive trusts
    [ ] Version 3.0
        * Added ability to choose functions before runtime
        * Cleaned up get-ouperms output
    [ ] Version 2.5
        * Bug fixes to version check for 2012R2 or greater specific checks
    [ ] Version 2.4
        * Forked project
        * Added Get-OUPerms, Get-LAPSStatus, Get-AdminSDHolders, Get-ProtectedUsers and Get-AuthenticationPoliciesAndSilos functions
        * Also added FineGrainedPasswordPolicies to Get-PasswordPolicy and changed order slightly
    [ ] Version 2.3
        * Added more useful user output to .txt files (Cheers DK)
    [ ] Version 2.2
        * Minor typo fix
    [ ] Version 2.1
        * Added check for null sessions
    [ ] Version 2.0
        * Multiple Additions and knocked off lots of the todo list
    [ ] Version 1.9
        * Fixed bug, that used Administrator account name instead of UID 500 and a bug with inactive accounts timespan
    [ ] Version 1.8
        * Added check for last time 'Administrator' account logged on
    [ ] Version 1.6
        * Added Get-FunctionalLevel and krbtgt password last changed check
    [ ] Version 1.5
        * Added Get-HostDetails to output simple info like username, hostname, etc...
    [ ] Version 1.4
        * Added Get-WinVersion version to assist with some checks (SMBv1 currently)
    [ ] Version 1.3
        * Added XML output for GPO (for offline processing using grouper https://github.com/l0ss/Grouper/blob/master/grouper.psm1)
    [ ] Version 1.2
        * Added check for modules
    [ ] Version 1.1
        * Fixed bug where SYSVOL research returns empty
    [ ] Version 1.0
        * First release