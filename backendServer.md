 <!-- import filesystem from "fs"
 import http from "http" -->
 import express from "express"
 import cors from "cors" 
  
  express()
  .use(cors(/* {origin: "http://localhost:5143"} */))
  .get("/countries", (req, res) => { // ezt a localhost:3000/countries-en érhető el
      res.json(data2);
    })
    .listen(3000);