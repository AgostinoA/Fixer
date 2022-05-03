From notify-desktop --help:

    Usage: notify-desktop [OPTION...] <SUMMARY> [BODY]
    
    Options:
       -r, --replaces-id=ID        Specifies the notifications ID that will be replaced
       -u, --urgency=LEVEL         Specifies the urgency level (low, normal, critical)
       -t, --expire-time=TIME      Specifies the timeout in milliseconds to expire the notification
       -a, --app-name=APP_NAME     Specifies the app name for the icon
       -i, --icon=ICON             Specifies an icon filename or stock icon to display
       -c, --category=TYPE         Specifies the notification category

ID of sent notification is written into standard output.

Examples:
    
    notify-desktop "Minimal notification"
    
    notify-desktop --icon=call-start "Incoming call"
    
    notify-desktop -i down -u low "Low urgency" "Body of low urgency notification"
    
Example bash functions that use --replaces-id option can be found in doc/ directory.
    
