# Component Hierarchy

**AuthFormContainer**
 - AuthForm

**HomeContainer**
 - Home
  * MovieIndex

**MoviesContainer**
 - MovieHeader
  * MoviePlay

**SearchResultsContainer**
 - Search

**MovieIndex**
 - MovieIndexItem
  + MovieDetail

**Search**
- SearchResultsContainer


## Routes

|Path   | Component   |
|-------|-------------|
| "/sign-up" | "AuthFormContainer" |
| "/sign-in" | "AuthFormContainer" |
| "/home" | "HomeContainer" |
| "/home/movie/:movieId" | "MovieContainer" |
| "/home/notebook/:notebookId/note/:noteId" | "NotebookContainer" |
| "/home/search-results" | "SearchResultsContainer"
| "/search" | "Search" |
