# Music Playlist Optimization Using Binary Integer Linear Programming

This project implements a music playlist generation approach based on Binary Integer Linear Programming (BILP).
The objective is to generate personalized playlists by maximizing user preference scores while satisfying predefined constraints on playlist duration and genre diversity.

The experiments use a filtered version of the AMBAR dataset, containing user-track preference information, track durations, and genre classifications.

https://github.com/davidcontrerasaguilar/AMBAR.git


## Experimental Configurations

Six experimental configurations are evaluated using different playlist duration intervals and minimum genre requirements.

| Experiment | Duration (seconds) | Minimum genres |
|---|---:|---:|
| E1 | 1200–1800 | 3 |
| E2 | 1200–1800 | 5 |
| E3 | 1800–2400 | 3 |
| E4 | 1800–2400 | 5 |
| E5 | 2400–3000 | 3 |
| E6 | 2400–3000 | 5 |

Each configuration is evaluated across 20 users, resulting in 120 optimization instances.

The experiments evaluate:

- Optimal preference scores.
- Playlist duration.
- Number of selected songs.
- Average preference per selected song.
- Genre diversity.
- Solver execution time.
- Optimization success and feasibility.


## Dataset

The project uses a filtered version of the AMBAR dataset.

The optimization input requires the following information:

| Attribute | Description |
|---|---|
| User ID | Unique user identifier |
| Song ID | Unique track identifier |
| Preference score | User preference for a track |
| Duration | Track duration in seconds |
| Genres | Associated genre categories |

The original dataset is not included in the repository. Place the required processed dataset in the corresponding data directory before executing the experiments.

