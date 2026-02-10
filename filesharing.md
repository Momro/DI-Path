# File Sharing

## NextCloud

- Good replacement for Google drive / one drive/Dropbox
- self-hosted and managed service
- how do you edit files on mobile device? -> collabora

## app
- nextcloud app
- for editing files: requires additional plug in/addon/docker, like onlyoffice or collabora (has separate app) 

### nextcloud self-hosted

#### tipps

```
$ sudo cat nextcloud/config/config.php | grep over
  'overwrite.cli.url' => 'http://nextcloud.domain.tld',
  'overwriteprotocol' => 'https',
```

see https://help.nextcloud.com/t/log-on-screen-hang/113564

#### collabora
be aware!
```
    environment:
      - "aliasgroup1=https://nextcloud.domain.tld:443"
```
it is wrong here https://collabora-online-for-nextcloud.readthedocs.io/en/latest/install/ 

found the solution here https://ask.linuxmuster.net/t/nextcloud-wechsel-von-eingebautem-auf-externen-collabora-server-keine-verbindung-zum-server/10404/4

### nextcloud managed

- price per month in €, all for 10 users
  - 100gb: 5€
  - 500gb: 7€
  - 2000gb: 10€

e.g. here: https://www.hosting.de/nextcloud/managed-nextcloud/

migration path from Google Drive and Dropbox


## Seafile


## Owncloud

Targets enterprises over private use 

## Syncthing

Good for synchronising files and folders, eg keepass file, or backup all photos from phone to storage/NAS.
