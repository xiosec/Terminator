# Invoke-Terminator


[![xiosec - Terminator](https://img.shields.io/static/v1?label=xiosec&message=Terminator&color=blue&logo=github)](https://github.com/xiosec/Terminator)
[![stars - Terminator](https://img.shields.io/github/stars/xiosec/Terminator?style=social)](https://github.com/xiosec/Terminator)
[![forks - Terminator](https://img.shields.io/github/forks/xiosec/Terminator?style=social)](https://github.com/xiosec/Terminator) [![GitHub release](https://img.shields.io/github/release/xiosec/Terminator?include_prereleases=&sort=semver)](https://github.com/xiosec/Terminator/releases/)
[![License](https://img.shields.io/badge/License-GPL-blue)](#license)
[![issues - Terminator](https://img.shields.io/github/issues/xiosec/Terminator)](https://github.com/xiosec/Terminator/issues)

Terminator is a powershell script that terminates protected processes such as [anti-malware](https://learn.microsoft.com/en-us/windows/win32/services/protecting-anti-malware-services-) and `EDRs` through the [gmer](http://www.gmer.net/) driver.

* in-memory
* HVCI bypass

# Usage

```powershell
<#
----------------------------
        Terminator

github : github.com/xiosec
twitter: twitter.com/xiosec
----------------------------

* Arguments
    * -ServiceName
    * -ProcName
    * -ProcId
    * -driverPath
#>

Invoke-Terminator -ServiceName terminator -ProcName MsMpEng 
```
# Example
In this example, we kill the `MsMpEng` process, which is related to the `antimalware service`.
![MsMpEng](assets/MsMpEng.png)

# Links

[gmer64.sys](https://www.loldrivers.io/drivers/7ce8fb06-46eb-4f4f-90d5-5518a6561f15/)

[Blackout](https://github.com/ZeroMemoryEx/Blackout)

# License 

Released under GPL-3.0 by [@xiosec](github.com/xiosec)