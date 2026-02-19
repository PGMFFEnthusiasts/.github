# Enter the Bradyverse

Running your own Touchdown server has never been so easy! We've pre-configured everything,
custom Brady patches and all for your usage.

### Requirements

- Docker (at the bare minimum)
- Knowledge on how to expose your server to the network (if you want that)

You can opt to either run the server from inside docker with the bundled java25 runtime, or if you want to run it straight
on your local machine (also useful for development) you can use the dump mode.

### Steps (docker)

1. Run the server:

   ```sh
   # You can change the -v parameter from ./data to wherever you want to store the data!
   docker run --rm -it -p 25565:25565 -v ./data:/server -e STANDALONE=true ghcr.io/pgmffenthusiasts/bradyverse-backend:latest
   ```
2. Connect and have fun!

### Steps (local)

1. Dump the server:

   ```sh
   # You can change brady-server to anywhere you want to store the server files
   docker run --rm -v ./brady-server:/server ghcr.io/pgmffenthusiasts/bradyverse-backend:latest dump
   cd brady-server
   ```

2. Start the server

   ```sh
   # (in brady-server)
   ./start.sh
   ```

3. Connect and have fun!
