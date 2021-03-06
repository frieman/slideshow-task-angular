# slideshow-task-angular

Your task is to develop a Web APP that fetches and iterate over media files (images and videos) from NoviSign API. The app should display and play media items as a slideshow in a loop, with cross-fade transitions and display duration.

#### NoviSign api

1. Get playlist:

Inorder to get the  media files you need to fetch 'playlists' and extract the media files to display over the screen.
Create a  page where you can paste a 'screen key' (0f127773-529f-4ff8-b211-af9e5c22a5bc) with that screen key you will be able to fetch the playlist and media files. After pasting the screen key user will be able to press 'play' button and play the playlist and media files.

Note:
- The playlist might be empty.
- There can be more then one playlist on screen.

In your app you can use the following 'screen key':
```
https://test.onsignage.com/PlayerBackend/screen/playlistItems/0f127773-529f-4ff8-b211-af9e5c22a5bc
```
Response E.g:
```JSON
{
  "screenKey": "0f127773-529f-4ff8-b211-af9e5c22a5bc",
  "breakpointInterval": 0,
  "playlists": [
    {
      "channelTime": 0,
      "playlistItems": [
        "fileKey": "pixabayImage-1518843.jpg",
        "creativeKey": "b1f1b49b-46b8-49ef-8177-309d28128bf7.jpg",
      ]
    }
  ]
}
```

2. Get media files:

In order to fetch the media file you should call NoviSign's API with the relevant file key.
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
How would you have implement the Bonus question? (If you hadnt implmented it :) )

Answer the question in an Answers.txt file

# Good luck!
