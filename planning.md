# Planning

## MVP Requirements

For singers: 
1. Accessible by browser on computer
2. Can find rehearsal track (ie by entering a code provided by the director)
3. Can identify self as a discrete user
   * low-security option: by providing a username/email which the director does not have to approve
4. Can listen to the composite track so far as many times as desired
5. Can record rehearsal attempt while listening to the track
   * No option to mute the track, actually
6. Upon completing first recording, it is automatically saved to the track files as username.wav
   * Upon completing subsequent recordings, it is automatically saved and overwrites the previous file
7. After listening, can still listen to composite track (including self)
8. At any time, can export the composite track as an audio file

For directors:
1. Accessible by browser on computer
2. Can create rehearsal track
3. Can add password to rehearsal track to use as director
4. Can export a track code to distribute to singers (aka a short url)
5. Can add the first recording, which is expected to be a piano accompaniment
6. Can listen to the composite track so far as many times as desired
7. At any time, can export the composite track as an audio file
8. At any time, can export a zip of the composite track plus individual recordings

## Future features
* Ability to "publish" a track (aka complete it to the point of releasing)
* Ability to restrict access to tracks, so strangers either have full access to the composite, 30s of listening, none, or not even the ability to see recent updates
* Home page which shows feed of recent rehearsal tracks and recent published tracks
* Choir entity which has at least one organizer but may or may not have a director (aka member-led choir)
* Ability to follow choirs, directors, or singers for their posts to show up in feed
* Profile page for choirs, directors, and singers for their public posts to be displayed
* Ability to restrict choir membership (must request/be invited to join) as the default
* Season entity which is a grouping of rehearsal tracks related to 1 or more choirs (ie fall season, Christmas season, 2021 season, etc)
* Starting out tips for directors (ie, recommendation to meet with accompanist in person to record video of the accompanist and director together)
* Export all composite tracks for one season (helpful to download tracks before meeting with singers in a call)
* Ability to start a new version of a track (such as if the director and accompanist change the base recording to have a different tempo/different nuances/better recording environment/etc; or if the singers need to start from scratch because old mistakes are still tripping people up on the recording)
* Ability to connect track files to file sharing system (Google Drive, GitHub, etc) for personal storage/backup/export
* Section entity to group singers into parts
* Ability to export the composite track for a single section
* More advanced: ability for singers to switch sections within a single song
* Settings for default sections of singers on main choir/season page which can be overriden for individual tracks
* Advanced feature: progress release (release a version of the track that has the first week through the final week of rehearsals, so the sound gradually gets better and better until the end)
* Make sure singer never experiences lag due to network by pulling from source before recording and pushing to source after finishing recording
* Settings file to individually decrease or increase the volume of any singers (intended to be used for differences in recording equipment/environment, but might also be used to balance volume between loud singers and soft singers)
* Ability to listen to only your section
* Ability for director/accompanist to create optional section rehearsal tracks (ie just Alto notes on piano, no accompaniment or other parts)
* Personal preference setting: when listening to composite track for rehearsal purposes, include my own voice or not?
* Weird idea: benefits for the "sight singer" group who records before others in their section
* Ability to tap a button while listening to add measure marks to the track
* "Breakout group" related to the rehearsal track which includes a smaller part of the rehearsal track which singers can attempt in a short amount of time while muted in a call with the director
* Track power ups/recommendations: add section groups, add measure tags, add director video, add rehearsal instrumental track, add individual section rehearsal instrumental track, add performance instrumental track, add text (lyrics) like subtitles, assign singers to sections
* Ability for director to programmatically choose the length of silence at the beginning of tracks
* After a singer records, ability to review their recording before uploading it
* In review, ability to compare their recording against:
  * The section
  * Their previous recording
  * The instrumental track
* Ability to try recording again and scrap recent recording
* Weird idea: after recording, director can programmatically choose a length of time to add to the track to let the singers talk to each other (ie the first sightreader says "Oof that was rough", the second singer tells a joke, the third singer laughs, the fourth singer says "How did you all finish rehearsing so fast?", etc) - I guess this would only work if the upload you send is final, otherwise someone might say something that sparks discussion and then they overwrite their file later, so it could work if the director enables a restriction so that members can only submit once per rehearsal period of days (although they can record and review as much as they want)
