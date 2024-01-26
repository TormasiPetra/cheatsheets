import http, { IncomingMessage } from "http"

const requestListenerFunction = (req: IncomingMessage) => {
    console.log(req.url)
}

http.createServer(requestListenerFunction).listen(3000) //akkor fut le a fn, amikor érkezik a http request a 3000-es porton keresztül

