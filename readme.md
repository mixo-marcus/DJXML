# DJXML

DJXML is an open format to import & export between DJ Software.

You own your DJ Library.  Let's keep it that way.

## Contribute

We're looking for contributors to help:
- Spread the word
- Define the metadata
- Test the XML and XSD
- Build libraries

## More Info

Project Website: [www.djxml.com](http://www.djxml.com)

## DJXML v1.0.1
```
- DJXML: DJXML Version Number
-- Software: Name and version of the software that exported the XML
-- Library: Number of tracks in the library


---- Track
----- TrackID
----- TrackName
----- Album
----- Artist
----- Remixer
----- Producer
----- Bpm
----- BitRate
----- Colour
----- Comments
----- DateAdded
----- DiscNumber
----- Genre
----- SubGenre
----- SubSubGenre
----- Grouping
----- Key
----- Kind
----- Label
----- Location
----- Mix
----- PlayCount
----- Rating
----- Remixer
----- SampleRate
----- Size
----- Tonality
----- TotalTime
----- TrackNumber
----- Year
----- Energy
----- Lossless
----- OriginalFormat
----- Pressing
----- Riddim
----- KeywordTags
----- PurchasedFrom
----- PurchaseLink   
     
------- Beatgrid
--------- StartTime
--------- Duration
--------- BeatType

------- CuePoint
--------- Name
--------- Type
--------- Start
--------- End
--------- Num
--------- Red
--------- Green
--------- Blue


-- Playlists: List of playlists with track IDs

--- Playlist
----- PlaylistName
----- TrackCount
------- TrackID (one entry for each track in playlist)
```


