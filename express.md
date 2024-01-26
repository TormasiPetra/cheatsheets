npm i express

in ts: 
    import express from "express"
    
const server = express()
server.use(express.static("public"))

server.get("data/all")