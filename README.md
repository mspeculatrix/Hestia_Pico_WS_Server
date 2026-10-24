# HESTIA: Pico WebSocket Server

This is MicroPython code to create a WebSockets server on a Raspberry Pi Pico 2W.

The idea is to create a communications hub on the Hestia robot, with WebSockets over wifi as the main comms channel.

The wifi connection and WebSocket functionality are in a class. As this is in a separate file, make sure you upload both `main.py` and `ws_server.py` to the Pico.

The WebSockets code supports multiple clients because ... why not? Output to the clients consists of broadcasting the same messages to all those currently connected.

There are, in fact, two ways of communicating with the Pico. There's WebSockets (of course) and a CLI via the Pico's USB. Responses from the Pico get sent to both channels.

## SUPPORT THIS PROJECT

If you find this project in any way interesting or useful, you could consider [buying me a coffee](https://ko-fi.com/zolachrome).
