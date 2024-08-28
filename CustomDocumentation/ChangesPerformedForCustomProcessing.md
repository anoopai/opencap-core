1. Use custom OpenSim model

```
# Check if shoulder model.if 'shoulder' in sessionMetadata['openSimModel']:
    suffix_model = '_shoulder'
elif 'NHE' in sessionMetadata['openSimModel']:
    suffix_model = '_NHE'
else:
    suffix_model = ''
if 'shoulder' in sessionMetadata['openSimModel']:
    suffix_model = '_shoulder'
elif 'NHE' in sessionMetadata['openSimModel']:
    suffix_model = '_NHE'
else:
    suffix_model = ''
```

2. Added utilsServer.py

```


newMetadata= {'openSimModel': 'LaiUhlrich2022_NHE','filterfrequence' = 4}    changeSessionMetadata(session_id,newMetadata)
```



    try:

    isGait=detectGaitAllVideos(mkrSpeedList,allMarkerList,confSyncList,markers4Ankles,sampleFreq)

    except:

    isGait=False

    print('Detect gait activity algorithm failed.')

    ifisGait:

    isGait=False
