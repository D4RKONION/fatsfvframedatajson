# FAT - SFV Frame Data JSON
This is the exact SFV frame data JSON file that [FAT](https://fullmeter.com/fat) and [FATOnline](https://fullmeter.com/fatonline) use. The frame data itself is mostly kept up to date by [@HatsonFGC](https://twitter.com/HatsonFGC) and to a lesser extent [@D4RK_ONION](https://twitter.com/d4rk_onion) (me), [@Arlieth](https://twitter.com/Arlieth), [@Frostdiener](https://twitter.com/Frostdiener) and BananaCyclone.

## The Spreadsheet
The information is created on [this google sheet](https://docs.google.com/spreadsheets/d/1nlbWon7SYhhO5TSpNx06qQrw2TRDEZ85HQrNherXioY/edit#gid=1311003467) which I then pull together into this JSON. If you want to report an error, please do so on [this discord](https://discord.gg/9BK8hHS). As I do not manually edit this file, pull requests or created issues are pointless. No, I probably wont give you spreadsheet edit access!


## JSON format
The JSON is formatted as follows:
```
{
    "character1": {
        "moves": {
            "normal": {
                "move 1": {
                    "stat1": 23,
                    "stat2": true,
                    ...
                },
                "move 2": {
                    "stat1": 4,
                    "stat2": false,
                    ...
                }
                ...
            },
            "vtOne": {
                "move 2": {
                    "stat1": 3,
                    "stat2": false,
                    ...
                }
                ...
            },
            "vtTwo": {
                "move 1": {
                    "stat1": 67,
                    "stat2": true,
                    ...
                },
                ...
            }
        "stats": {
            "stat1": 1000,
            "stat2": 3,
            ...
       }
   },
   ...
}
            
            
```
Please note: only moves that change in VT1/2 exist inside that objects. However all characters have a VT1/2 object, even if it's empty. If you'd like to see what each key/value pair means, you can check the first sheet on the spreadsheet [here](https://docs.google.com/spreadsheets/d/1nlbWon7SYhhO5TSpNx06qQrw2TRDEZ85HQrNherXioY/edit#gid=1311003467)

## Using this file
You are free to use this file in your own projects as per the license [here](https://github.com/D4RKONION/fatsfvframedatajson/blob/master/LICENSE). Basically give us credit!