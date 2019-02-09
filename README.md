# Computational Musicology
_What makes music religious?_


Github Page of the repository for the 2019 Computational Musicology course at the UvA

---

## Week 1

Music has been around since the history of mankind. However, where most of today's music tends to be used for personal entertainment, it was often used to give praise to deities. But are there any musicological properties of a piece of music that make it specifically suitable for religious purpouses? Bach himself sometimes re-used his 'pagan' music for religious purposes and vice versa giving an important role to lyrics. However, we also know that Bach was a master in the writing of baroque [affective](https://en.wikipedia.org/wiki/Doctrine_of_the_affections) music, indicating a carefull use of pitch, volume, tibre, and time for bringing music to it's purposes. So, even if there is some overlap between musical sound of pagan en religious music, there might be some aspects which fit just better for one of them.

To be able to answer the research question one has to compare religious music with
non-religious music. This is implemented in `R` using the `spotifyr` module which gathers data from two types of playlist: _religious_ and _non-religious_. Both corpuses are more usefull for machine learning purposes, as for example classification, if they contain many songs. Therefore, a set of different playlists which tend to be typically religious or non-religious has been made. Depending on the results, the religious playlists could be split up further to detect if there are any difference between different religions. Differences are measured between contemporary music lists but could be further expanded to more classical oriented music.

        See [this page](https://github.com/MBWhitestone/Computational_Musicology/blob/master/README.md) for a correct rendering of the tables

####  Religious Playlists
| Title                          | ID                     | Songs |
| ------------------------------ | ---------------------- | ----- |
| Religious Songs                | 1Lfv5hpiBqtxHIlaeUo8TS | 44    |
| Top Christian Contemporary     | 37i9dQZF1DWUileP28ODwg | 58    |
| Top Christian                  | 37i9dQZF1DXcb6CQIjdqKy | 66    |
| Christian Playlist for 2017    | 37i9dQZF1DXcb6CQIjdqKy | 391   |
| Islamic / Nasheeds             | 1dNteyophghoFsbO3lCULn | 67    |
| Islamic Song                   | 3SxT23r9nc6M1Ew2xrVpaV | 108   |
| Sanskrit / Hindu Mantra Chants | 6RLNAQJoR5OUAl5lyA8YJJ | 133   |
| Buddhist Meditation Songs      | 3c4AduB9UOrxkfdW0Nh2hA | 270   |
| Top Jewish Music               | 05Um5tgwbBWNAikYlwCId6 | 255   |

Which makes up a total of **1298** _unique_ religious songs.*


#### Non-religious Playlists
| Title              | ID                     | Songs |
| ------------------ | ---------------------- | ----- |
| Top 2017           | 1DoUPHRIAC6YbEPiDf8IOd | 99    |
| Today's Top Hits   | 37i9dQZF1DXcBWIGoYBM5M | 50    |
| TOP 2019           | 208tdAvqyrtssZFKLktwkx | 43    |
| Top Tracks of 2018 | 37i9dQZF1DX1HUbZS4LEyL | 100   |
| Top of the Charts  | 7b2rMhQyuX3vkgQz2umhdV | 107   |
| Top allertijden    | 1nwCwjYUStN0xvoSmSgS9M | 785   |

Which makes up a total of **1186** _unique_ non-religious songs.*  

        Notice that it is hard to tell whether all these top-songs are really non-religous.

\* Using the `distinct` function from `R`.

## First Findings

The following plot should still be normalized, colorised and is missing indications of the standard deviations, which will be added once the authors R-skills are at the right level:
![](./doc/firstmeans.png)

Anyway, there are already some interesting findings visible like the difference in danceability of religious and non religious music. On average religious music is less danceable but more lively compared to non-religious music. Regarding standard deviations the speechiness is low but has a very high deviation meaning that there is little to say about the speechiness of religious and non religious songs _on average_.
