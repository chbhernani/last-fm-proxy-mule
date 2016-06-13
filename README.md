# Proxying Last.FM API with Mulesoft Platform #

Utilizing [Last.FM API](http://www.last.fm/api/), this proxy brings the artist details or track details in JSON format, depending of what parameter is sent. When only "artist" parameter is sent, an JSON with artist details is returned. When both parameters "artist" and "track" are sent, a JSON with track details is returned.

2 parameters are received:
	- artist (required): The artist name 
	- track (optional): The track name
