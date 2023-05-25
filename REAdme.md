# shopbag-backend

proccess to add files:- 
1. npm init -y 
2. npm i json-server cors
3. npm i json-serve
4. add db.json and paste  all data
5. create server.js  and add ----->
###
const jsonServer = require('json-server')
const server = jsonServer.create()
const router = jsonServer.router('db.json')
const middlewares = jsonServer.defaults()
const port =process.env.PORT ||8080

server.use(middlewares)
server.use(router)
server.listen(port, () => {
  console.log('JSON Server is running')
})

###
process to deploy on render-
1.  login render through github
2.  click on new 
3.  select web service
4.  give api name
5.  and click on deploy
6.  it will take some time to deploy
