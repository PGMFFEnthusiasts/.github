# PGMFFEnthusiasts

Running your own Touchdown server has never been so easy! We've pre-configured everything,
custom Brady patches and all for your usage.

### Requirements

- Docker (at the bare minimum)
- Knowledge on how to expose your server to the network (if you want that)

### Steps

1. Run the server:

   ```sh
   # You can change the -v parameter from ./data to wherever you want to store the data!
   docker run --rm -it -p 25565:25565 -v ./data:/server ghcr.io/pgmffenthusiasts/bradyverse-backend:standalone
   ```
2. Connect and have fun!
