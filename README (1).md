# Proxy Switcher — Fabric 1.21.4

Client-side Minecraft mod that routes remote Minecraft connections through a selected SOCKS5 proxy.

## Build
Requirements: Java 21 and Gradle 8.x/9.x compatible with the pinned Fabric Loom.

From this folder:
- Windows: `gradlew.bat build`
- Linux/macOS: `./gradlew build`

The finished mod is in `build/libs/`, using the `-sources.jar` only for source code; install the other jar.

## Install
1. Install Fabric Loader for Minecraft 1.21.4.
2. Install Fabric API for 1.21.4.
3. Put the built `proxy-switcher-1.0.0.jar` into `.minecraft/mods`.
4. Launch the Fabric 1.21.4 profile.
5. Press P to open Proxy Switcher.
6. Add a SOCKS5 proxy and select it before connecting.

Java 21 is required for Minecraft 1.21.4.

The server sees the network address of the SOCKS5 proxy, not the local address, provided the proxy is actually used and does not leak it through another connection.
