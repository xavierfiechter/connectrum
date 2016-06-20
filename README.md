# Connectrum

## Stratum (electrum-server) Client Protocol library

Use python3 to be a client to the Electrum server network. It makes heavy use of
`asyncio` module and newer Python 3.5 keywords such as `await` and `async`.

This is meant to be a mostly-clean room implementation, but isn't.

For non-server applications, you can probably find all you need
already in the standard Electrum code and command line.


## Setup

    virtualenv -p python3 ENV
    (activate ENV)
    pip install -r requirements.txt
    cd examples
    python3 explore.py


## TODO List

- be more robust about failed servers, reconnect and handle it.
- connect to a few (3?) servers and compare top block and response times; pick best
- some sort of persistant server list that can be updated as we run
- type checking of parameters sent to server (maybe)?
