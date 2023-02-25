# gateserver
A small script that handles account authentication and session validation for LoonaPS microservices.

### Modules used
- [Chalk](https://npmjs.com/package/chalk) - A beautiful color logging library. Makes crash and exit logs look good.
- [andesite](https://github.com/LoonaPS/andesite) - A library with a set of definitions and tools used for LoonaPS made into a TypeScript/JavaScript module. 
- [ws](https://npmjs.com/package/ws) - A library that can interact with a Websocket server. Used for connecting to dbgate.

### how do you set it up?
1. Clone the Github Repository via Git Bash

```powershell
git clone https://github.com/LoonaPS/gateserver.git
```

2. Extract and open the repository in the Terminal

```powershell
# Assuming that you are in Windows/Linux
cd gateserver
```

3. Fix the configuration files.
- A dbgate instance is required to be able to run this microservice. Provide the endpoint IP address for where the dbgate is hosted, leave the value to `127.0.0.1` if the dbgate instance is hosted locally with gateserver. An authentication password is important to make sure your dbgate instance is secure and restricted to endpoints who has the password, make sure you haven't left that out yet.

```powershell
npm install --save-dev
npm run start
```