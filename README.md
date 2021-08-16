# The-First-Responder-Toolkit

```Learned from: SANS, EC-Council```

## Volatile Information Colection Commands

###### For Windows:
> date /t & time
> 
>doskey /history
> 
>net statistics server
> 
>netstat -ab
>
>net File
>
>Openfiles
>
>tasklist
>
>netstat -ano
>
>net sessions
>>      net session [\\ComputerName] [/delete]
>
>wmic
>>Examine Auto Start processes:
>>>     wmic /node:<remote-ip> /user:<username> startup list full
>>
>>Find who is logged on to a computer's console:
>>>     wmic /node:<remote-ip> /user:<username> ComputerSystem Get UserName
>>
>>Query local user accounts:
>>>     wmic /node:<remote-ip> /user:<username> useraccount list full
>>
>>Find the path to a specific running executable and its parent process (for all, leave off ?where name='):
>>>     wmic /node:<remote-ip> /user:<username> process where get ExecutablePath,parentprocessid
>>
>>Find command line invocation of a specific executable as well as the creation time for the process (for all, leave off ?where name='). Reference this [Microsoft TechNet article](https://docs.microsoft.com/en-us/previous-versions/tn-archive/ee156576(v=technet.10)?redirectedfrom=MSDN) for converting the time:
>>>     wmic /node:<remote-ip> /user:<username> process where get name,processid,commandline,creationdate
>
>ListDLLs (SysInternals)
>>      listdlls [-r] [-v | -u] [processname|pid]
>
>>      listdlls [-r] [-v | -u] [processname|pid] 
>
>PsList.exe (SysInternals)
>>       Pslist-x
>
>pmdump.exe (for memory dumps)
>
>psloggedon.exe (SysInternals)
>>      psloggedon [-] [-l] [-x] [\\computername | username]
>
>PsFile (SysInternals)
>
>LogonSessions.exe
>>      logonsessions [-c[t]] [-p]
>
>Free Clipboard Viewer https://freeclipboardviewer.com/es/
>
>
>

For Linux
>uptime
>
>top
>
>ps
>
>pstree
>
>who
>
>who am i, who -uH
>
>who -all/-a
>
>last
>
>lastlog
>
>w
>
>lld
>
>
