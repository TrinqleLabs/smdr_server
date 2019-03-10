# SMDR server

This is fake SMDR server, emulating Panasonic PBX SMDR server behavior. It
provides access to SMDR data over telnet. It can be used to test SMDR
analyzing software.

Calls data is taken from sample file. Samples isn't included at this moment,
but I will upload one later.

## How to run

`python3 smdr_server.py -f sample.log`

### Command-line options

`-f, --file` — path to sample log file. Required argument.  
`-H, --host` — server IP address. Default `localhost`  
`-P, --port` — default `6023`  
`-p, --password` — prompt for a password to change it
from default `pccsmdr`. Clients are prompted for this password
to access SMDR data.
