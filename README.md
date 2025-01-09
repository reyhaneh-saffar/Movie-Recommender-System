# Movie Recommender System

## Overview
This project implements a **content-based movie recommender system** that suggests a list of movies to a user based on their movie preferences. The system works on the principle that users are likely to enjoy movies with similar characteristics to those they already like.

## Methodology
To achieve the recommendations, the system follows these key steps:
1. **Data Analysis**: Prepare and merge datasets to extract relevant information.
2. **System Development**: Build a content-based recommender using movie features such as cast, keywords, and genres.
3. **Testing**: Evaluate the system by generating movie recommendations for users.

## Highlights

### Data Preparation
  - Merging datasets and resolving column type mismatches.
  - Cleaning and preprocessing key columns (`cast`, `keywords`, `genres`) for analysis.

### Building the Recommender
- **Feature Extraction**: Combine key features into a single "soup" string for each movie.
- **Efficient Similarity Search**: Use **MinHashLSHForest** to efficiently find similar movies based on content.

### Recommendation Process
1. User inputs their ID.
2. The system retrieves the user's favorite movies (rated at least 4).
3. Similar movies are identified and ranked based on relevance.
4. Top 10 recommendations are displayed.

## Key Features
- **Content-Based Filtering**: Focuses on movie characteristics rather than user behavior.
- **Scalable Design**: Uses efficient data structures to handle similarity searches.
- **User-Friendly Output**: Provides personalized recommendations in a clear and concise manner.
