# Article.FICalloutsFixGwy
FI Callouts Fix Gateway server

To get this running:

1. Make sure you have Java 8 available in your classpath.
1. Download this project as a ZIP file (it will be named `Article.FICalloutsFixGwy-master.zip`).
1. Unzip the file where ever you want it installed.
1. Go to the `config` directory under the install directory and edit the `gateway.cfg` file.
    * Change `SocketConnectHost=[REMOTE_FIX_SERVER_HOST]` and `SocketConnectPort=[REMOTE_FIX_SERVER_PORT]` to the host/IP address and port of the remote ATRU FIX server.
    * Change `SenderCompID=[YOUR_SENDER_SESSION_COMP_ID]` to the appropriate Comp ID for your session.
    * Change `TCID=[YOUR_TCID]` to the appropriate TCID.
1. Save the file.
1. Go to the `bin` directory and run `start.bat` (Windows) or `start.sh` (Unix).
1. The Gateway server will start and you will automatically be connected to FIX session at the remote host:port for compid you configured.
1. To stop the FIX connection just exit or stop the Gateway server.





