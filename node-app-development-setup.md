# install node on developer workstation

https://nodejs.org/en/download/package-manager

node can be installed using the nvm 
first install the nvm
using nvm install node

```bash
# installs nvm (Node Version Manager)
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash

# download and install Node.js
nvm install 20

# verifies the right Node.js version is in the environment
node -v # should print `v20.13.1`

# verifies the right NPM version is in the environment
npm -v # should print `10.5.2`
````

ABOVE DID NOT work for me  on MAC with ZSH

used https://nodejs.org/en/download/prebuilt-installer  # this worked

3. mkdir <node-app> ; cd node-app
4. npm init 
5. npm install express 
6. check the official express documentation
   npm install express --save
   https://expressjs.com/en/starter/installing.html


   app.js

   ```javascript
   const express = require('express')
const app = express()
const port = 3000

app.get('/', (req, res) => {
  res.send('Hello World!')
})

app.listen(port, () => {
  console.log(`Example app listening on port ${port}`)
})
   ```

   ```bash
   node app
   node app.js
   ```