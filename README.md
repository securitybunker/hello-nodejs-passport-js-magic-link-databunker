# databunker-nodejs-example

This is an example of the nodejs login and signup page built with the following technologies:

* Passport.js http://www.passportjs.org/
* Magic.link https://magic.link/
* Databunker https://databunker.org/

**This project was originally based on Magic.Link Nodejs example:**

https://codesandbox.io/s/github/MagicLabs/example-nodejs

An in-depth review of the Databunker' [Secure Session Storage](https://databunker.org/use-case/secure-session-storage/).


# Prerequisites

## 1. Start Databunker service:

For the purpose of testing you can use the following command to start **databunker**:

```docker run -p 3000:3000 -d --rm --name dbunker securitybunker/databunker demo```

For production installation, follow the Databunker installation guide: https://databunker.org/doc/install/


## 2. Set environment variables

Make sure that you have the following environment variables in place:
```
export DATABUNKER_URL=http://localhost:3000/
export DATABUNKER_TOKEN=DEMO
export MAGIC_PUBLISHABLE_KEY=pk_test_AAAA
export MAGIC_SECRET_KEY=sk_test_BBBB
```

# Install all dependencies

```npm install```

# Run the service

```
node app.js
```
