# Simple Single Page Soundboard (JSON version)

The original [Simple Soundboard](https://github.com/digitalcolony/Simple-Soundboard) required PHP to load MP3 files from a directory to be loaded onto the Soundboard. This version requires no server-side code and the sound files can be loaded from a remote web server.

All you need is a JSON file that follows this format.

```json
{
  "files": [
    {
      "name": "A Stench of Cow Manure... - Jim Mandich",
      "mp3":
        "https://archive.org/download/neil-rogers-show-soundboard/A-Stench-of-Cow-Manure.mp3"
    },
    {
      "name": "Absolutely Correct Sir - Neil Rogers/Old Bridge Dude",
      "mp3":
        "https://archive.org/download/neil-rogers-show-soundboard/Absolutely-Correct-Sir.mp3"
    }
  ]
}
```

The name field has both the title of the audio track and the artist seperated by a dash. Artist name is optional.

## Hosting Audio on Archive.org

You could host the audio files anywhere you like, but for this project, I used archive.org. Once I had a page created with all the audio drops I wanted on my Soundboard, I used a NodeJS tool I wrote called [JSON builder for Archive.org](https://github.com/digitalcolony/archive-json-builder) that builds the JSON file.

## Resources

1. The Soundboard uses [Ballon.CSS](https://kazzkiq.github.io/balloon.css/) for the mouseover tooltips.
1. The styling for the soundboard buttons were created with help from [CSS Button Generator](http://css3buttongenerator.com/).

## More Info

You can also review the README on the [original version](https://github.com/digitalcolony/Simple-Soundboard) for more information and ideas.
