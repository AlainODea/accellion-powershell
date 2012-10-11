accellion-powershell
====================

Accellion API Client Written in Powershell 

PURPOSE
-------
Proof of concept example of how to use Accellion's APIs.

Everything here can easily be adapted to other programming languages.

USAGE
-----
1. Launch Powershell
2. Copy/Paste contents of AccellionAPIs.ps1 into the shell
3. Edit and copy/paste the following to get a file listing

```powershell
function Run-Example
{
    $hostname="accellion.example.com"
    $applicationId="1234"
    # this is NOT the secretKey from the invite email
    # it is found under APIs in Admin
    $loginSecret="1234567890abcdef1234567890abcdef"
    $uid="user.name@example.com"
    $domain = "c1s1"
    Get-AccellionFiles $hostname $applicationId $loginSecret $uid $domain
}
Run-Example
```