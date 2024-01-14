Install and configure qbittorrent-nox
=========

This role installs and configures qbittorrent-nox for my server.

Role Variables
--------------



Example Playbook
----------------

```yaml
    - hosts: servers
      roles:
         - { role: qbittorrent_nox, qbittorrent_nox_web_password: password123,
             qbittorrent_nox_torrent_path: /share/video-share/Torrents }
```

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
