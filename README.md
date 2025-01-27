# jupyter-tunnel
A script to connect to remote jupyter server using ssh tunnel.

```
 $ curl -o ~/.local/bin/jupyter-tunnel.py https://raw.githubusercontent.com/apuapaquola/jupyter-tunnel/master/jupyter-tunnel.py
 $ chmod +x ~/.local/bin/jupyter-tunnel.py
```

When called, jupyter-tunnel:
+ discovers available ports and makes a ssh tunnel to the remote host
+ calls jupyter lab on the remote host
+ calls firefox on the local host passing a URL to connect to jupyter server

<pre>
jupyter-tunnel.py [-h] [--host HOST] [--dir DIR] [--user USER]
                         [--default-tunnel-port DEFAULT_TUNNEL_PORT]
                         [-p SSH_PORT]

optional arguments:
  -h, --help            show this help message and exit
  --host HOST
  --dir DIR
  --user USER
  --default-tunnel-port DEFAULT_TUNNEL_PORT
  -p SSH_PORT, --ssh-port SSH_PORT

</pre>
