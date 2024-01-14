Install and configure qbittorrent-nox
=========

This role installs and configures qbittorrent-nox for my server.

Role Variables
--------------

```qbittorrent_nox_torrent_path``` should be set to the path where torrents should be downloaded to.

```qbittorrent_nox_interface``` can be set to the interface that should be used qBittorrent (for example vpn interface).

```qbittorrent_nox_web_username``` can be set to the username that should be used by the web interface.

```qbittorrent_nox_port``` can be set to the port that should be used by the web interface.

With ```qbittorrent_nox_user_name``` and ```qbittorrent_nox_user_group``` you can set the user and group that should be used by qBittorrent.

And ```qbittorrent_nox_user_uid``` and ```qbittorrent_nox_user_gid``` can be set to the uid and gid used by the user

Example Playbook
----------------

```yaml
    - hosts: servers
      roles:
        - { role: qbittorrent_nox, qbittorrent_nox_torrent_path: /share/video-share/Torrents,
             qbittorrent_nox_interface: tun0 }
```

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
