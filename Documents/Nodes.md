<center>

| **Event Name** 	|   **Elements**  	  |       **Description**         |
|:--------------:	|:------------------: |:----------------------------: |
|   ready 	      | name, resumed       | Event of the node connection. |
|   error         | name, error 	      | Event of the node error.      |
|   close         | name, code, reason  | Event of the node close.	    |
|   disconnect    | name, players, move | Event of the node disconnect.	|
|   debug         | name, reason	      | Event of the node debug.      |
</center>


## Event
```
Zyroka.shoukaku.on("ready", (name) => {
 console.log("node connected")
});
```
