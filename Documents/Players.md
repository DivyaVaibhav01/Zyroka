<center>

| **Event Name** 	  |   **Elements**  |       **Description**         |
|:----------------: |:--------------: |:----------------------------: |
|   trackStart	    | player, track   | Event of the track start.     |
|   trackEnd        | player, track	  | Event of the track end.       |
|   queueEnd        | player          | Event of the queue end.	      |
|   PlayerClosed    | player, data    | Event of the player close.	  |
|   trackException  | player, data	  | Event of the track exception. |
|   PlayerUpdate    | player, data	  | Event of the player update.   |
|   trackStuck      | player, data	  | Event of the track stuck.     |
|   trackError      | player, error   | Event of the track error.     |
|   PlayerResumed   | player          | Event of the player resumed.  |
|   PlayerDestroy   | player	        | Event of the player destroyed.|
|   PlayerCreate    | player	        | Event of the player create.   |
</center>

# PlayerQueue
```
const zyrokaPlayer = zyroka.createPlayer({
      guildId: guild.id,
      voiceId: voiceChannel.id,
      textId: channel.id,
      shardId: guild.shardId,
      volume: 100,
      deaf: false
});

const songInfo = {
  "title": zyrokaPlayerr.queue[0].current.info.title,
  "uri": zyrokaPlayerr.queue[0].current.info.uri,
  "image": zyrokaPlayerr.queue[0].current.info.artworkUrl,
  "source": zyrokaPlayerr.queue[0].current.info.sourceName
};

const requesterInfo = {
    "name": zyrokaPlayerr.queue[0].current.requester.username,
    "id": zyrokaPlayerr.queue[0].current.requester.id,
}
```

## Event
```
zyroka.on("trackStart", (player, track) => {
const channelId = player.textId;
});
```
