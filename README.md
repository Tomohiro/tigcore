tigcore
================================================================================

[TweetIrcGateway](http://www.misuzilla.org/Distribution/TweetIrcGateway/) core dll management tool.



Requirements
--------------------------------------------------------------------------------

Use `/bin/sh`. Tested on OSX.


Installation
--------------------------------------------------------------------------------

Download to your executable path.

    $ cd $HOME/bin
    $ curl -LO https://raw.github.com/Tomohiro/tigcore/master/tigcore
    $ chmod +x ./tigcore


Usage
--------------------------------------------------------------------------------

Check the list of downloadable `TwitterIRCGatewayCoreDLL`

    $ tigcore versions
    ...
    TwitterIrcGatewayCore.dll-20120817-Debug
    TwitterIrcGatewayCore.dll-20120817-Debug2
    TwitterIrcGatewayCore.dll-20120817-Debug3
    TwitterIrcGatewayCore.dll-20130306

Download `TwitterIRCGatewayCoreDLL`

    $ cd /path/to/your/TweetIrcGateway/
    $ tigcore install TwitterIrcGatewayCore.dll-20130306


Enable the DLL. Then restart the TweetIrcGateway service.

    $ tigcore use TwitterIrcGatewayCore.dll-20130306
    Created symbolic link to /path/to/your/TwitterIRCGateway/TwitterIrcGatewayCore.dll


Last, restart the TweetIrcGateway service.


LICENSE
--------------------------------------------------------------------------------

&copy; 2013 Tomohiro TAIRA.
This project is licensed under the MIT license.
See LICENSE for details.
