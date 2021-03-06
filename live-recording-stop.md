# API Method: /api/live/recording/stop

Stop recording from a live video stream.


### Parameters

<table class="pretty">
  <tr><th>Parameter</th><th>Description</th></tr>
  <tr><td><tt>live_id</tt> <small>(required)</small></td><td>The ID for the stream for which you want recording to stop.</td></tr>
</table>

    

### Permission level 

The minimum required [permission level](index#permission-level) is:

    write


### Example XML Response

    <response status="ok" permission_level="write" 
      message="The stream has stopped recording" cached="0">
      <upload_token>live-678j35g34jh54309</status>
    </response>

### Example JSON Response

    {
      "status": "ok", 
      "message":"The stream has stopped recording",
      "permission_level":"write",
      "cached":"0",
      "live":{"upload_token": "live-678j35g34jh54309"},
      "p": "1",
      "size": "1",
      "site": { ...},
      "endpoint": "/api/live/stop-recording"
    }