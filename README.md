# zabbix

I have recently tried creating a new Media Type in Zabbix, and got multiple error messages while set up.
It looks the official version of YAML maintained on zabbix git repository doesn't seem to work for everyone. (atleast for me)
So, I have modified it to make it work on my machine. Adding it here in case anyone else run in to same issue.


# Instructions

1. Download the "telegram_mediatype.yaml" file to your local machine.
2. Go to Zabbix Webconsole, navigate to "Administration > Media Types" and then import the YAML from step above.
3. Once the template is imported, then follow remaining instructions from below link.
   https://git.zabbix.com/projects/ZBX/repos/zabbix/browse/templates/media/telegram/README.md
   
   
# Possible errors with using official version of script.
1. Invalid tag "/zabbix_export/version": unsupported version number (In my case, I am using Zabbix 5.2 version, so I change the version number to 5.2, version: '5.2')
2. TypeError: undefined not callable (property 'log' of [object Object]) at [anon] (duktape.c:65639) internal at [anon] (function:55) preventsyield
3. ...
