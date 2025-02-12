# Healthcare Patient Intake AI

## How to run agent

Store your Twilio, Vocode, Deepgram, Ngrok, Azure Speech, and OpenAI API/Authentication keys in a local `.env` file.

Launch your Ngrok host with the following command.

```properties
ngrok http 3000
```

With Docker installed, launch the agent with Docker build and compose.

```properties
docker build -t vocode-telephony-app .
```
```properties
docker-compose up
```

Finally, make sure your Twilio phone number is connected by webhook to your Ngrok url.  Then call your number and you'll have an AI agent available to collect your intake information!
