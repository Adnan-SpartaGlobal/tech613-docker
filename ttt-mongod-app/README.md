# How to run these two compose files

Both methods assume that you are in the `ttt-mongodb-app` folder

## Manual
1. `cd` into the folder `ttt-mongod-app-manual`
   ```
   cd ttt-mongod-app-manual
   ```

2. Use the Docker command
   ```
   docker compose up -d
   ```

   - This allows you to open up any and all containers created in the `docker-compose.yml` file
   - The containers are based on the images they are given
   - The composition runs in detacthed mode, due to the `-d`

3. Run the command 
   ```
   docker exec -it tech613-adnan-app-container node seeds/seed.js
   ```
   This **seeds** data into the mongodb to then be displayed in the tictactoe web-app

4. Close all containers when you are done
   ```
   docker compose down
   ```


## Automatic
1. `cd` into the folder `ttt-mongod-app-automatic`
   ```
   cd ttt-mongod-app-automatic
   ```

2. Use the Docker command
   ```
   docker compose up -d
   ```

   - This allows you to open up any and all containers created in the `docker-compose.yml` file
   - The containers are based on the images they are given
   - The composition runs in detacthed mode, due to the `-d`
   
   **Note:** The data should already be **seeded** so no need to run `docker exec`

3. Close all containers when you are done
   ```
   docker compose down
   ```


