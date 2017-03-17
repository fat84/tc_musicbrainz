# MusicBrainz

MusicBrainz **APPLICATION ONLY**
Bring your own external PostgreSQL database.

*Note* to avoid conflicts, the search server is 5080 on the host redirected to 8080 in the container. 8080 is a commonly used port.

# Sample Setup
**DO NOT USE, BROKEN CURRENTLY.**
docker create -p 5000:5000 -p 5080:8080 -v /media/config/musicbrainz:/config -v /media/musicbrainz:/home/musicbrainz --name testnzbget docker.io/rootwyrm/tc_nzbget:latest
