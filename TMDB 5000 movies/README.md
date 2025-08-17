Dataset Summary & Structure

Shape: 4,803 movies, with 4 columns: movie_id, title, cast, crew.
Integrity: No missing values in any columns.
Features:
Cast: JSON-formatted list of actor credits per movie.
Crew: JSON-formatted list of crew credits per movie.

Key EDA Insights

1. Most Frequent Actors
   
2.Analysis extracted all actor names from all movies, counting appearances.
Top 15 most frequent actors: (Presented as a horizontal bar chart in your notebook)
Notable names with high counts (such as Samuel L. Jackson, Tom Cruise, etc.) frequently appear in blockbusters and franchise films.

3. Most Frequent Directors
Extracted each movie's director from the 'crew' field.

Top 15 most frequent directors: (Also shown as a horizontal bar chart.)
Common directors include Steven Spielberg, Ridley Scott, and others well-known for their prolific output.

3. Distribution of Cast Size (per Movie)
Calculated the number of credited cast members per movie.
Visual Insight: The histogram shows most movies have a cast size between 5 and 30, with a peak around 10–20.
Some movies have very large casts, but these are rare; majority of titles use more modest ensembles.

Data Preparation Workflow

Used ast.literal_eval to safely parse the JSON-like 'cast' and 'crew' columns from strings into Python objects for further analysis.
Ensured each record was properly converted so that aggregation and counting would be accurate.

Data Types & Missing Values
movie_id: int64
title, cast, crew: object (cast & crew as string-encoded JSON lists)

No missing data in these primary columns.

Author:Sabin Shah
contact:sabinshah619@gmail.com
