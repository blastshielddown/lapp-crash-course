# Lightning App Crash Course

This is an example media store powered by Lightning payments. The accompanying tutorial/guide can be found on [Medium](https://medium.com/@rheedio/a-crash-course-in-lightning-app-development-part-deux-51a8e48a4540)

## Tools

[Polar](https://lightningpolar.com/) is required.

## Configuration

Copy lnd's gRPC protocol from [here](https://raw.githubusercontent.com/lightningnetwork/lnd/master/lnrpc/lightning.proto) and place in the `backend` dir.

References to the lnd `admin.macaroon`, `tls.cert`, and `host:port` need to be filled in before starting the backend server.

Media files go in `backend/static`. Thumbnails go in `client/public/assets`.

Metadata for media is set in the `client/App.js` file.

## Run

### Express Server (backend)
Run `node app.js` from the `backend` dir.

### React Client (client)
Run `npm start` from the `client` dir.

Open [http://localhost:3000](http://localhost:3000) to view in the browser.

