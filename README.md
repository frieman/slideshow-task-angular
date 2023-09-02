# slideshow-task-angular

Your task is to develop a Web APP that fetches and iterate over media files (images and videos) from NoviSign API. The app should display and play media items as a slideshow in a loop, with cross-fade transitions and display duration.

#### NoviSign api

1. Get playlist:

Inorder to get the  media files you need to fetch 'playlists' and extract the media files to display over the screen.
Create a  page where you can paste a 'screen key' (294d453d-9176-44c2-9db9-f2759031e8e4) with that screen key you will be able to fetch the playlist and media files. After pasting the screen key user will be able to press 'play' button and play the playlist and media files.

Note:
- The playlist might be empty.
- There can be more then one playlist on screen.

In your app you can use the following 'screen key':
```
https://test.onsignage.com/PlayerBackend/screen/playlistItems/294d453d-9176-44c2-9db9-f2759031e8e4
```
Response E.g:
```JSON
{
  "screenKey": "294d453d-9176-44c2-9db9-f2759031e8e4",
  "breakpointInterval": 0,
  "playlists": [
    {
      "channelTime": 0,
      "playlistItems": [
        "duration": 10,
        "creativeKey": "6daa1483-4fe0-4424-9d82-1ec1c3423a33.jpg",
      ]
    }
  ]
}
```

2. Get media files:

In order to fetch the media file you should call NoviSign's API with the relevant creative key.
E.g:
```
https://test.onsignage.com/PlayerBackend/creative/get/b1f1b49b-46b8-49ef-8177-309d28128bf7.jpg
```
### Bonus 
Check for playlist updates and display accordingly, without starting it over again.

### Last thing
##### What we anticipate to see in the  app:

1. Write the app with Angular and Typescript.
2. Write unit tests
3. Use design patterns that allows flexible code structure, showing anticipation for evolution and new features 
4. Cut corners, but not to the point where the structure vanishes
5. Conventional coding style
6. README file and Reasonable comments (where needed)

##### Question:
1. How would you have implement the Bonus question? (If you hadnt implmented it :) )
2. How would you support offline mode? E.g in case the computer reboot and returns without internet.

Answer the question in an Answers.txt file

# Good luck!
