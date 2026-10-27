TryTP (Fabric, Minecraft 1.21.4, client-side)

BUILD
  1. Install JDK 21 and Gradle (or copy the gradle wrapper from the official Fabric example mod).
  2. In this folder run:  gradle build
  3. Put build/libs/trytp-1.0.0.jar in .minecraft/mods (with Fabric API).

USE
  /trytp <player>   wait for them to turn TPA on, then send /tpahere <player>
  /trytp cancel     stop waiting
  /trytp reload     reload config

CONFIG  (.minecraft/config/trytp.json)
  patterns  - regexes for the server message that means "TPA is on". Edit to match your server.
  command   - what gets sent, default "tpahere %player%"
  delayMs   - delay before sending, default 50
