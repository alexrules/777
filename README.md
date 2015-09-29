<!DOCTYPE html>
<!--
    Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
    with the License.  You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing,
    software distributed under the License is distributed on an
    "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
     KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
-->
<html>
    <head>
        <meta charset="utf-8" />
        <meta name="format-detection" content="telephone=no" />
        <!-- WARNING: for iOS 7, remove the width=device-width and height=device-height attributes. See https://issues.apache.org/jira/browse/CB-4323 -->
        <meta name="viewport" content="user-scalable=no, initial-scale=1, maximum-scale=1, minimum-scale=1, width=device-width, height=device-height, target-densitydpi=device-dpi" />
        <link rel="stylesheet" type="text/css" href="css/index.css" />
        <title>Taxi in Riga</title>
    </head>
    <body>
        <div class="app">
            <h1>Book a Taxi in Riga</h1>
            <div id="deviceready" class="blink">
                <p class="event listening">Connecting to tracking server</p>
                <p class="event received">Done</p>
            </div>
        </div>

        <div id="ready"></div>
        <script type="text/javascript" src="cordova.js"></script>
        <script type="text/javascript" src="js/index.js"></script>

        <script type="text/javascript">
            app.initialize();
            // Wait for Cordova to load
            //
            document.addEventListener("deviceready", onDeviceReady, false);

        

                function onError(error) {
                    alert('code: '    + error.code    + '\n' +
                            'message: ' + error.message + '\n');
                }

            // Cordova is ready
            //
            function onDeviceReady() {
                // navigator.geolocation.getCurrentPosition(onSuccess, onError);
                // document.getElementById("ready").innerHTML = "I'm ready !!";

                // navigator.geolocation.getCurrentPosition(x, onError);


               var ref = window.open('http://bookingtaxiriga.com', '_blank', 'location=yes');
      
               ref.addEventListener('exit', function() { alert(event.type); });

            }







        </script>
    </body>
</html>
