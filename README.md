# 3 Decades of Medical Drama Politics
Scraping scripts from long-running medical dramas (ER, Scrubs, House, Grey's Anatomy, The Good Doctor) to analyze the morals that they advocate for.

## Datasets: 
*All in CSV format*

Shows:
- show_id: The IMDb ID of the show (primary key)
- title: Title as listed on IMDb
- description: Short description as listed on IMDb

Episodes:
- ep_id: The IMDb ID of the episode (primary key)
- title: Title as listed on IMDb
- season: Season number the episode was in
- ep_num: Episode number of the season
- air_date: The original air date of the episode
- description: Short description as listed on IMDb
- imdb_rate: The IMDb rating of the episode
- show_id: The IMDb ID of the show (foreign key)

Writers:
- writer_id: The IMDb ID of the writer (primary key)
- name: The full name of the writer as listed on their IMDb profile

Writing Credits: (Associative Entity meant for joining writers to episodes)
- ep_id (foreign key)
- writer_id (foreign key)

To be added: Scripts dataset either with TXT files of transcripts connected to episode IDs or text objects stored in a larger table
