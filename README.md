# Candy Simply-Fi

The device sends a broadcast UDP heartbeat in every ~7 seconds to `255.255.255.255` port `55555`.
This way you can detect whether its turned on.


You can read the status of the appliance on the local network with this simple script:
[candy_getstatus.py](candy_getstatus.py)

## Output examples

### Device status

http://&lt;device ip&gt;/http-read.json?encrypted=1
```
{
        "statusTD":
{"StatoWiFi":"0",
                "StatoTD":"1",
                "CodiceErrore":"0",
                "Pr":"2",
                "PrPh":"0",
                "RemTime":"150",
                "DryLev":"2",
                "Time":"0",
                "Rapido":"0",
                "Opt1":"0",
                "Opt2":"0",
                "Opt3":"0",
                "Opt4":"0",
                "Opt5":"0",
                "Opt6":"0",
                "Opt7":"0",
                "Opt8":"0",
                "Refresh":"0",
                "CleanFilter":"0",
                "WaterTankFull":"0",
                "DryingManagerLevel":"0",
                "DelVal":"0",
                "DoorState":"1",
                "RecipeId":"NULL",
                "CheckUpState":"0"
        }
}
```

### Statistics

http://&lt;device ip&gt;/http-getStatistics.json?encrypted=1

```
{
        "statusCounters":{
                "s1":"0",
                "s2":"0",
                "s3":"0",
                "s4":"0",
                "s5":"0",
                "s6":"0",
                "s7":"0",
                "s8":"0",
                "s9":"0",
                "s10":"0",
                "s11":"0",
                "s12":"0",
                "s13":"0",
                "s14":"0",
                "s15":"0",
                "s16":"0",
                "s17":"0",
                "s18":"0",
                "s19":"0",
                "s20":"0",
                "s21":"0",
                "s1t":"0",
                "s2t":"0",
                "s3t":"0",
                "s4t":"0",
                "s5t":"0",
                "s6t":"0",
                "s7t":"0",
                "s8t":"0",
                "s9t":"0",
                "s10t":"0",
                "s11t":"0",
                "s12t":"0",
                "s13t":"0",
                "s14t":"0",
                "s15t":"0",
                "s16t":"0",
                "s17t":"0",
                "s18t":"0",
                "s19t":"0",
                "s20t":"0",
                "s21t":"0",
                "sCottonBone":"0",
                "sCottonStore":"0",
                "sCottonHang":"0",
                "sCottonIron":"0",
                "sSynthBone":"0",
                "sSynthStore":"0",
                "sSynthHang":"0",
                "sSynthIron":"0",
                "sCottonT60":"0",
                "sCottonT120":"0",
                "sCottonT180":"0",
                "sCottonTMax":"0",
                "sSynthT60":"0",
                "sSynthT120":"0",
                "sSynthT180":"0",
                "sSynthTMax":"0"
        }
}
```

