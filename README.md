# Proxying Last.FM API with Mulesoft Platform #

Utilizing [Last.FM API](http://www.last.fm/api/), this proxy brings the artist details or track details in JSON format, depending of what parameter is sent. When only "artist" parameter is sent, an JSON with artist details is returned. When both parameters "artist" and "track" are sent, a JSON with track details is returned.

2 parameters are received:
- artist (required): The artist name
- track (optional): The track name
	
### Set Up and Run the Example in Anypoint Studio

Complete the following procedure run this project in your own instance of Anypoint Studio.

1. Open the project in Anypoint Studio.
2. In the Package Explorer pane in Studio, right-click the project name, then select Run As > Mule Application. Studio runs the application and Mule is up and kicking!
4. Open your Web browser.
5. In the address bar, type URLs like following: 
	- http://localhost:8081/details?artist=ARTIST (Ex: [http://localhost:8081/details?artist=U2](http://localhost:8081/details?artist=U2))
	- http://localhost:8081/details?artist=ARTIST&track=TRACK (Ex: [http://localhost:8081/details?artist=U2&track=One](http://localhost:8081/details?artist=U2&track=One))
6. Press enter to elicit a response from application. 
