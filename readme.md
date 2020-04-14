# DJXML

DJXML is an open format to import/export between DJ Software.

You own your DJ Library.  Let's keep it that way.

## Contribute

We are looking for contributors to help:
- Contact DJ Software manufacturers for support
- Define the Track criteria for DJXML
- Develop the XML/XSD format

Thank you in advance for your help :-)

## More Info

Project Website: [www.djxml.com](http://www.djxml.com)

Supported by (so far!): [www.mixo.dj](http://www.mixo.dj)


## DJXML v1.0.0
```
- DJXML: DJXML Version Number
-- Software: Name and version of the software that exported the XML
-- Library: Number of tracks in the library


---- Track
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
----- TrackID
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
----- Count
----- Entries
----- KeyType
----- Type
```


