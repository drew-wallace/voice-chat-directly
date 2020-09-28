# voice-chat-directly

Tiny server so people can voice chat with me directly

Based on [https://github.com/emannion/webrtc-audio-video](https://github.com/emannion/webrtc-audio-video)

Future feature could be to use the WebAudioAPI like in this [https://github.com/webrtc/samples/tree/gh-pages/src/content/peerconnection/webaudio-input
](https://github.com/webrtc/samples/tree/gh-pages/src/content/peerconnection/webaudio-input
)

## Setup the ssl cert
```
openssl genrsa -out webrtcwwsocket-key.pem 1024
openssl req -new -key webrtcwwsocket-key.pem -out webrtcwwsocket-csr.pem
openssl x509 -req -in webrtcwwsocket-csr.pem -signkey webrtcwwsocket-key.pem -out webrtcwwsocket-cert.pem
```