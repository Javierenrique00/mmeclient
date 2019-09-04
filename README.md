# MMECLient Documentation

MMeClient means Minio Media Client, and it is the complement of a Minio Music Server [here](https://github.com/Javierenrique00/minio_Music_Server).

MMeClient is a Android app (Free and without advertising also) that you can download in Google Play see, [MMeClient](https://play.google.com/store/apps/details?id=com.mundocreativo.javier.mmeclient&hl=en)

MMeClient reads the Minio Music Server Index file, and can find, download and play files that are stored in a Minio server or public cloud storage. ( Amazom s3, Google storage, Azure Backblaze B2 and other public anonimous storage)

_MMeClient Screenshot_
![ScreenShoot](./pictures/Screenshot_20190904-152246.png)



Instrucctions to use MMeClient app.

## 1- Configuring the Media Storage

When you enter for the first time to MMeClient the first thing to do is configuring the access to the Media Storage.

You have to select the "spanner" in the upper right of the screen in orther to configure settings, including the access to the Media Storage.
![ScreenShoot](./pictures/Screenshot_20190904-152400.png)

There are some parameters to configure. You can leave the defaults.

**Max songs in cache:** default(30) Is the max number of songs that the app keeps downloaded (ocupiying storage in the android device) when you select play songs of a directory or a group of songs. If you choose a big number the Android device can get run out of storage space.

**Predownload songs:** default(2) Is the number of songs that the app try to download in advance in a queue of songs before the song needs to be played.

**Only Internal Player:** default(Yes) The app has an internal player for audio files. This internal player can load music to the play queue with one touch of a directory or group of selected files. But you can also use an external player like (Vanilla Music) or VLC or other external player. The difference is that for an external player you can only add music one file at the time. In the internal player you can add music to the queue songs on any number of selected songs or directories.

note:in Vanilla music is possible to play a song, to add a song to a queue or XXXX.

Then push the button called **"New Server"**. With this button you can see 4 fields that you need to configure for adding a storage.
**Address path field** The first field you need to put the full address where the storage is located, including the bucket. in the screenshoot the bucket is **test**.
Examples of address path are:
https://storage.googleapis.com/mystorage

https://f001.backblazeb2.com/file/mybucket

**Index file field** This is the second field, is the name of the index file in the above path.
**Enable Field** Default is disabled, but if you selected, it try to download the index file. Leave enable to see the files in the storage.
**Password field** If your storage is encrypted write the password in this field. (Optional) and then select **enable** to read the encrypted index file.

You can have multiple servers or storages but only you can downloaded media files if they are **enabled**.



