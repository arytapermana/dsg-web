---
title: Build Your Own Minecraft Multiplayer Server
date: 2021-05-23 00:00:00 +08:00
layout: ampstory
cover:
  title:Build Your Own Minecraft Multiplayer Server
  subtitle: A little IT background required
  background: https://ik.imagekit.io/dsg/thumb_RSrSNhvh5.jpg
  backgroundblur: true
pages:
- layout: thirds
  middle: "<h2>You need Minecraft Server and also Ngrok</h2>"
- layout: vertical
  top: "<h2>Run the following command to start Minecraft Server</h2><br/><p>java
    -jar server.jar --world m-server</p>"
  background: https://ik.imagekit.io/dsg/m-server_aAVedRiqJ.png
  backgroundblur: true
- layout: vertical
  top: "<h2>Save the port that appears in the log, the default port usually</h2><br/><p>port=
    25565</p>"
  background: https://ik.imagekit.io/dsg/m-server_aAVedRiqJ.png
  backgroundblur: true
- layout: vertical
  top: "<h2>Enable local port forward to Ngrok server</h2><br/><p>ngrok tcp
    -region ap 25565</p>"
  background: https://ik.imagekit.io/dsg/m-server-2_1__6bW9zX72j.png
  backgroundblur: true
- layout: vertical
  top: "<h2> Just join the server...</p>"
  image: https://ik.imagekit.io/dsg/m-server-3_hQYpbxa-I.png
---

