# Proxying Last.FM API with MuleSoft Anypoint Platform™ #

 Built with [MuleSoft Anypoint Platform™](https://www.mulesoft.com/) and utilizing [Last.FM API](http://www.last.fm/api/), this proxy brings the artist details or track details in JSON format, depending of what parameter is sent. When only "artist" parameter is sent, an JSON with artist details is returned. When both parameters "artist" and "track" are sent, a JSON with track details is returned.

Two parameters are received:
- artist (required): The artist name
- track (optional): The track name

### Assumptions

This guide assumes that you have downloaded and installed [Anypoint Studio](https://www.mulesoft.com/lp/dl/studio). 

### Set Up and Run application in Anypoint Studio

Complete the following procedure run this project in your own instance of Anypoint Studio.

1. Import **proxy-last_fm.zip** in Anypoint Studio (**File > Import... > Anypoint Studio > Anypoint Studio generated Deployable Archive (.zip) > select proxy-last_fm.zip > Finish**).
2. In your application in Studio, click the **Global Elements** tab. Double-click the **HTTP Listener Configuration** global element to open its **Global Element Properties** panel. Change the contents of the **port** field to required HTTP port (e.g. 8081) and save.
3. In the Package Explorer pane in Studio, right-click the project name, then select **Run As > Mule Application**.
4. Open your **Web browser**.
5. In the address bar, **type URLs** like following: 
	- http://localhost:8081/details?artist=ARTIST (Ex: [http://localhost:8081/details?artist=U2](http://localhost:8081/details?artist=U2))
	- http://localhost:8081/details?artist=ARTIST&track=TRACK (Ex: [http://localhost:8081/details?artist=U2&track=One](http://localhost:8081/details?artist=U2&track=One))
6. Press enter to elicit a **JSON response** from application.

### Accessing deployed application in CloudHub

If you want, can access this application in CloudHub. Change the value of the params for other results.
- Ex: http://proxy-last-fm.cloudhub.io/details?artist=Coldplay
- Ex: [http://proxy-last-fm.cloudhub.io/details?artist=Coldplay&track=Paradise
