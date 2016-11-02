# ---flix *name to be changed*


##Minimum Viable Product
---flix *name to be changed* is a web application inspired by Netflix built using Ruby on Rails
and React/Redux.  By the end of Week 9, this app will, at a minimum, satisfy the
following criteria with smooth, bug-free navigation, adequate seed data and
sufficient CSS styling:

- [ ] Hosting on Heroku
- [ ] New account creation, login, and guest/demo login
- [ ] Smooth, bug-free navigation, adequate seed data and sufficient CSS styling
- [ ] Production README

- [ ] 'Movies' (Commercials)
  -Access various movies (pick/play)
- [ ] Ratings
  - See average rating for a movie
  - Rate a movie
- [ ] Search


## Implementation Timeline

### Phase 1: Backend setup and Front End User Authentication (2 days)

**Objective:** Functioning rails project with front-end Authentication

- [X] New Rails project
- [X] User model/migration
- [X] Back end authentication (session/password)
- [X] StaticPages controller and root view
- [X] Webpack & react/redux modules
- [X] APIUtil to interact with the API
- [X] Redux cycle for frontend authentication
- [X] User signup/signin components
- [X] Blank landing component after signup/signin
- [ ] Style signup/signin components
- [X] Guest Login
- [ ] Review phase 1

### Phase 2: Series Model, API, and components (2 days)

**Objective:** Series can be created, read, edited and destroyed through the API.

- [ ] Series model
- [ ] Seed database with a small amount of test data
- [ ] CRUD API for series (SeriesController)
- [ ] JBuilder views for series
- Series components and respective Redux loops
  - [ ] SeriesIndex
    - Will be primary portion of app
      * Included in 'browse', 'mylist' and 'search'
  - [ ] SeriesIndexRow
    - Each row in the index that implements 'wrap-around' scrolling
  - [ ] SeriesIndexItem
    - Ratings
    - Play current episode
  - [ ] SeriesDetailPane
      - SeriesDetail
      - SeriesOverview
      - SeriesEpisodes
  - [ ] Seed series

### Phase 3: Episode Model, API, and components (3 days)

**Objective:** Episodes can be created, read, edited and destroyed through the API.

- [ ] Episode model
- [ ] Seed database with a small amount of test data
- [ ] CRUD API for episodes (EpisodesController)
- [ ] JBuilder views for episodes
- Episodes components and respective Redux loops
  - [ ] EpisodeIndex
    - Nested in SeriesIndexItem::SeriesEpisodes
    - Implement 'wrap-around' scrolling
  - [ ] EpisodeIndexItem
  - [ ] EpisodeShow
    - Be able to watch an episode through YouTube API
  - [ ] Seed episodes within series

### Phase 4: Reviews (2 day)

**Objective:** Reviews belong to series that can be created, read, edited and destroyed through the API.

- [ ] Review model
- [ ] Seed database with a small amount of test data
- [ ] CRUD API for reviews (ReviewsController)
- [ ] JBuilder views for reviews
- [ ] Adding reviews requires a series
- Reviews components and respective Redux loops
  - [ ] ReviewsIndex
    - Preview shown in SeriesIndexItem::SeriesDetail

      - All reviews shown through Modal

  - [ ] ReviewForm
    - User can write own review in SeriesIndexItem::SeriesDetail
- [ ] Seed reviews

### Phase 5: Searching (1 day)

**Objective:** Be able to search for series by genre or title

- Search results will use presentation components of primary app (series & episodes) but will filter which series are sent

- [ ] Search model
- [ ] Seed database with a small amount of test data
- [ ] CRUD API for Search (SearchController)
- [ ] JBuilder views for Search

### Phase 6: My List (1 day)

**Objective:** Be able to create a list of series-to-watch that can be updated (added to & removed from)

- MyList will use presentation components of primary app (series & episodes) but will filter which series are sent

- [ ] MyList model
- [ ] CRUD API for MyList (MyListsController)
- [ ] JBuilder views for MyList
- [ ] Seed database with a small amount of test data

### Phase 7: Pagination / infinite scroll for Series Index (1 day)

**Objective:** Add infinite scroll to Series Index

- [ ] Paginate Series Index API to send 4 results at a time
- [ ] Append next set of results when user scrolls and is near bottom
- [ ] Style scroll components and transitions
- [ ] Ensure seed data demonstrates infinite scroll### Bonus

### Bonus
- [ ] Bonus: Sort movies by IMDB rating
- [ ] Bonus: Sort movies by actor
- [ ] Bonus: Search for actor's movies
- [ ] Bonus: MyList
  - Create a 'My List' to keep track of series-to-watch
  - Wrap-around Scroll
  - Series are organized by genre with a 'wrap-around' scroll
- [ ] Bonus: Scribble log in
