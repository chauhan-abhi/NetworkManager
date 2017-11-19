# NetworkManager
This app uses GCM Network Manager to make battery optimized network calls.

The app implements 2 types of network calls:
* With network connectivity, "NOW" requests are executed immediately and
  "WHEN BEST" requests are executed within about 30 seconds.
* Without network connectivity (turn Airplane Mode on), "NOW" requests fail and
  "WHEN BEST" requests remain pending and are executed when network connectivity returns (turn Airplane Mode off).

If a task is scheduled at a time when the device does not have network connectivity,
GCM Network Manager can hold on to that task and only execute it when network connectivity has returned.

# Snaps

<img src="https://github.com/chauhan-abhi/NetworkManager/blob/master/art/nonetwork.png" width="360" height="640">
<img src="https://github.com/chauhan-abhi/NetworkManager/blob/master/art/network.png" width="360" height="640">

# Libraries Used

* Recycler View
* Gson
* Commons.io


