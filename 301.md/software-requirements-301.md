# Software Requirements

- What is the vision of this product?
  - Our vision is to create an app that allows the user to search a band, and get a return of similar artists. The user can log in, and save artists that they have listened to or delete them.

- What pain point does this project solve?
  - Finding new music can be overwhelming. Our app gives the user a manageable amount of suggestions.

- Why should we care about your product?
  - This allows the user to seek out recommendations, unlike predetermined algorithms.

- IN - What will your product do
  - Describe the individual features that your product will do.
  - High overview of each. Only need to list 4-5
    - authenticate user with auth0
    - produce list of bands that are similar to the user's search query
    - save searches to database
    - display in a pleasing way, so user can scroll and save.

- OUT - What will your product not do.
  - It will not become a app
  - it will not be a music streaming service
  - will not turn into a social media

- Minimum Viable Product vs
  - What will your MVP functionality be?
    - User can search a band and get a return of 10 artists that are similar to that band. The user can scroll through a carousel of the returned bands. The user can delete the band and also favorite it and see a visual signal that you favorites that artist. 

- What are your stretch goals?
  - Being able to re-arrange favorite bands in the order of you're choosing.
  - favorites page
  - search by anything other than band ex: era, genre, location

- Stretch
  - What stretch goals are you going to aim for?
    - favorites page
    - rearranging your favorites

- Functional Requirements
  - Pages: About Us, Login, Search
  - User has ability to delete and favorite bands
  - ability to search api for new bands
  - Logout Button

- Dataflow
  [WWR](/301/WWR_project.jpg)

- Non-Functional Requirements
  - Authenticate user sign in with Auth0
    - Auth0 is an external authorization and authentication tool
  - Usability
    - a clean UI, understandable for the user
