# DJXML
Developer Integration Guide 

DJXML is a generic export from MIXO, combining libraries from popular DJ and music apps into a single XML file.

MIXO supports a wide variety of DJ and music apps, including Rekordbox 5, Rekordbox 6, Traktor, Serato, iTunes and more! The simple structure of DJXML contains all Folders, Playlists, Tracks, Metadata and Cues imported into or created in MIXO.

A single integration allows users from almost any DJ software to effortlessly migrate to your software. 

## More Info

Project Website: [www.djxml.com](http://www.djxml.com)

Encoding and Decoding of Special Characters

XML files are encoded on export (as are the XML/NML for Rekordbox / TRAKTOR / Virtual DJ)

That means that unsafe ASCII characters are converted:

```
& = &amp;
" = &quot;
< = &lt;
> = &gt;
```

Please note: apostrophes are not converted. These should be converted when parsing the XML file to the HTML entity (```&apos;```). 

This will allow parsing to complete successfully.

After parsing, HTML entities will need replacing in all metadata, cue names, folder names, playlist names and filePaths. 

## DJXML v2.0.0
```
- DJXML: DJXML Version Number
-- Software: Name and version of the software that exported the XML
-- Library: Number of tracks in the library


---- Track
----- Id
----- Title
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
----- MusicalKey
----- TotalTime
----- TrackNumber
----- Year
----- Energy
----- Lossless
----- Pressing
----- Riddim
----- KeywordTags
----- PurchasedFrom
----- PurchaseLink   
     
------- Beatgrid
--------- StartTime
--------- Bpm
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


-- Playlists: List of nested folders, playlists and playlist tracks (referencing TrackIDs)

--- Folder
----- Id
----- Name
----- Entries (number of sub folders or playlists)
----- ParentFolderId

------ Playlist
------- PlaylistName
------- Entries
------- Id
------- ParentFolderId

-------- PlaylistTrack
--------- TrackId
```


