![Flickr](https://live.staticflickr.com/65535/49770138256_8e54fdfaa0_b.jpg)

<p align="center">
    <h3>Real Time Message Protocol (RTMT Server) for OBS </h3>
</p>

## Deskripsi :
* Server RTMT untuk Menjalankan Stream Video dari OBS.

----------------------------------------------------------------------------------------------------

## Library :

| Library           | Package Instalation                                                               |
| ---------------   | --------------------------------------------------------------------------------- |
| Node Media Server | *npm install --save node-media-server*                                            |

--------------------------------------------------------------------------------------------------------------

## Source Pendukung :

* Applikasi Video Stream : ![OBS](https://obsproject.com/)
* Dokumentasi NMS : [NodeMediaServer](https://github.com/illuspas/Node-Media-Server#npm-version-recommended)
* Index.js 

  ```JSX
    const config = {
        rtmp: {
            port: 1935,
            chunk_size: 60000,
            gop_cache: true,
            ping: 30,
            ping_timeout: 60
        },
        http: {
            port: 8000,
            allow_origin: '*'
        }
    };

    var nms = new NodeMediaServer(config)
    nms.run();
  ```

