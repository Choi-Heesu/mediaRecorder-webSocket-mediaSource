# mediaRecorder-webSocket-mediaSource
------------

## Description

Browser to browser video chat testing without WebRTC.
How to Use the web socket server to send and receive data in real time.

The overall process will be like this:

1. Obtain media stream using `getUserMedia` to access webcams on the local computer.
2. `MediaRecorder` encodes media stream and converts it into blob data.(media segment)
3. Send blob data to the server via a web socket.(Blob data will be converted into arrayBuffer)
4. The server returns the data back to the client.
5. By using `appendBuffer`, appends the media segment to the SourceBuffer in MediaSource.


## Usage

#### Start the web socket server by `npm install` and `npm start`
```
$ cd backend
$ npm install
$ npm start
```

#### then start client side
```
$ cd frontend
$ npm install
$ npm start
```

#### open http://localhost:3000 in broswer

