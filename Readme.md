# weather-furenberger-com.herokuapp.com
[weather-furenberger-com.herokuapp.com](https://weather-furenberger-com.herokuapp.com)

Example of using react hooks to populate a map with state boundary clickability and then zip specific lookup of weather.

## Running

This uses an express server as well as the react SPA.

### Server (Heroku)
On the server (heroku) the application is built/bundled and served from express.

the heroku dyno runs a npm i for the server automatically

`heroku-postbuild' npm installs and builds the client application

When the dyno starts it funs the Procfile `node server/index.js`

### Localhost

The ideal set up for debugging is two terminals.  You can run one just like the server but then the logs only appear for the UI.  You could even run a third/fourth terminal with the tests too.

One Terminal (client)
`cd client && npm run start`

Second Terminal (server)
`npm run start` (or `npm run start:nodemon`)


You will need a .env file (make a copy of .env.fake and rename)

Get your mapbox token: https://www.mapbox.com/
Get your openweather token: https://openweathermap.org/
