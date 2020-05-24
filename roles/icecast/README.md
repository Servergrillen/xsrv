icecast
============

This role will install [Icecast](https://en.wikipedia.org/wiki/Icecast) server, a streaming media server. It can stream audio or video content (in many formats) over HTTP, making it accessible through a simple web browser or media player. This allows you to setup an [Internet Radio](https://en.wikipedia.org/wiki/Internet_radio) service.

A continuous playlist/stream will be generated from media files placed in the `PLAYLIST` directory on the server.

You can also use external sources such as another computer as the source of audio/video content, and let the Icecast server distribute it. [Here](https://github.com/quodlibet/quodlibet/issues/2795) is an example configuration for streaming from a media player to an Icecast server (Quodlibet > Pulseaudio > Icecast).

**Note**: currently only OGG audio files are supported in the playlist directory. Place your audio files in the `PLAYLIST/`  directory using SFTP, then run `./srv01 icecast-update` to reload the playlist. When listening to the stream in Firefox, track changes will cause playback to stop. Use VLC _Play network stream_ or another player for playback without stops between tracks.

**Note**: After updating the files in the playlist directory, you must run the playbook (at least with `--tags=icecast` for the noew playlist to be generated)

[![](https://i.imgur.com/gFv229u.png)](https://i.imgur.com/c7180pa.png)
[![](https://i.imgur.com/3wqkckz.png)](https://i.imgur.com/6GAjBB4.png)


Requirements
------------

This role requires Ansible 2.7 or higher.


Role Variables
--------------

See [defaults/main.yml](defaults/main.yml)


Dependencies
------------

None

Example Playbook
----------------


License
-------

GNU GPLv3

References
-----------------

- **https://en.wikipedia.org/wiki/Icecast**
- **https://icecast.org/**
- **https://icecast.org/apps/**
- **https://icecast.org/docs/**
- **https://icecast.org/ezstream/**
- **https://wiki.archlinux.org/index.php/Icecast**
- https://github.com/quodlibet/quodlibet/issues/2795
- https://hstuart.dk/2010/11/07/gstreamer-and-pulseaudio-to-a-squeezebox/
- https://icecast.org/docs/icecast-2.4.1/
- https://icecast.org/docs/icecast-2.4.1/basic-setup.html
- https://serverfault.com/questions/648669/icecast-and-apache-on-the-same-port-mod-proxy-mod-rewrite
- https://serverfault.com/questions/739178/how-to-set-up-an-automatic-failover-reverse-proxy-for-two-identical-icecast-mast
- https://wiki.archlinux.org/index.php/Icecast
- https://wiki.xiph.org/Icecast_Server
- https://wiki.xiph.org/Icecast_Server/known_https_restrictions
- https://wiki.xiph.org/Icecast_Server/known_reverse_proxy_restrictions
- **https://serverfault.com/questions/648669/icecast-and-apache-on-the-same-port-mod-proxy-mod-rewrite** patch to allow reverseproxy https://damiengarrido.wordpress.com/2015/03/22/icecast-reachable-behind-reverse-proxy/

