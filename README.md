# Audio-Fingerprinting-with-Python

This code is to recognise a five second recording, provided the original song is already in ur database i.e, if your computer has already "learnt" the song.

It is based on the fingerprint/hashing algoritm developed by Shazam Inc.

Before running the code, make sure u have the following already in your system:
1. Jupyter Notebook
2. MySQL: Create a database named "songsdb". After setting this as the default database, create three tables in it using the following code:-
                  CREATE TABLE rechashes(num INT AUTO_INCREMENT PRIMARY KEY, hashes VARCHAR(255), recoffset INT)
                  CREATE TABLE ref(song_id INT AUTO_INCREMENT PRIMARY KEY, Song_name VARCHAR(255))
                  CREATE TABLE songsource(hashval_ VARCHAR(255), song_id INT, offset_ INT)  
3. A good quality microphone to record noise-free audio.

While trying to read new songs into the database, try to cropped versions of the song(1-2 mins) rather than the standard 3-4 mins versions
