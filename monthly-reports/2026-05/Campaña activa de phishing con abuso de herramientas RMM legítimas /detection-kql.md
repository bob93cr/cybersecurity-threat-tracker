DeviceNetworkEvents
| where Timestamp > ago(30d)
| where RemoteUrl has_any (
    "gruta.com.mx",
    "server.cubatiendaalimentos.com.mx"
)
or InitiatingProcessFileName in~ (
    "SimpleHelp.exe",
    "ScreenConnect.ClientService.exe",
    "elev_win.exe"
)
| project Timestamp,
          DeviceName,
          RemoteUrl,
          InitiatingProcessFileName,
          InitiatingProcessCommandLine,
          InitiatingProcessAccountName
| order by Timestamp desc
