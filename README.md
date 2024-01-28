# DealMeIn

## Summary

A system for hosting and playing virtualised card cames.

### GameClient

A Blazor progressive web application that acts as the end-user interface for the hosted games.

### GameBroker

A .Net web API acting as a broker for the hosted games. Facilitates the registration of game servers with the broker, as well as game discovery for the game clients.

### GameServer

A .Net application using SignalR to host one or more game rooms for a specific game. 

This project uses is to be hosted in a Docker container, with the published `.dll` and asset files for a particular game injected.

One game server instance hosts one specific game.