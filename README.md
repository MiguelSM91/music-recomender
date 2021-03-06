# **music-recomender**


*Miguel Simón*

*November 2020, Barcelona*

### PROJECT DESCRIPTION
In this project I have developed a music recomender using web scrapping and spotify API.
I have generated several databases that will be called depending on the step of the flowchart we are.

  - Flowchart

  The system will take a song name as input.
  If the song is a actual hit it will retreive other actual hit.
  If the song is not a hit but it was a hit in the last decade it will retreive oher hit from that decade.
  The decade analysis will work for 70s, 80s, 90s and 00s too.
  If the input song was not a hit, the program will analyze the music features and it will retreive other song that meets the same features, based on a clustering.
  If for some reason the program is not able to get the song features it will automatically retreive other song from a bonus list composite by "songs that everybody knows" from spotify.

  - databases
    · Top 100 hits from billboard web (generated by web scrapping)
    · Top 1000 hits from 70s from billboard web (generated by web scrapping, year by year and the joined in a single df)
    · Top 1000 hits from 80s from billboard web (generated by web scrapping, year by year and the joined in a single df)
    · Top 1000 hits from 90s from billboard web (generated by web scrapping, year by year and the joined in a single df)
    · Top 1000 hits from 00s from billboard web (generated by web scrapping, year by year and the joined in a single df)
    · Top 1000 hits from 10s from billboard web (generated by web scrapping, year by year and the joined in a single df)
    · 1000 general songs organized by clustering (generated by spotify API)
    · 100 song taht everybody knows as a bonus list in case the system can not get the song features (generated by spotify API)

    - Organization
    This repository is composite by a "Data" folder with all the generated databases and a "Instructions" folder with the emails we got from out company partners with the starting point for this project. In addition, it has several python notebook files with the different steps I took to develop the project. The final version is in the "FINAL_recomendator" file.
