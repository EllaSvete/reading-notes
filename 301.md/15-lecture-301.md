# Auth0 lecture

## Lab 13

- Add Auth0 to frontend
- What is Auth?
  - authorization: what are you allowed to do
  - authentication: who are you
- Oauth
  - protocol for authentication
- Auth0
  - a company that uses Oauth protocol
- Process
  - Computer pins Auth0
  - Auth0 checks request legitimacy
  - comes back as ok or NOT ok
  - of comes back as ok token gets sent to server
  - server send to Auth0
  - Auth0 responds if is ok or not
  - server sends to client, heres the data you wanted
- auth0.com

- in index.js
- import ReactDOM
- in the ReactDOM.render()
- copy and paste Auth0Provider from website
- LoginButton.js: copied from auth.com
- LogoutButton.js: copied ^
- Profile.js: copied

- In .env
  - REACT_APP_AUTH_DOMAIN=auth domain
  - REACT_APP_AUTH_CLIENT_ID=copied from website
  - REACT_APP_AUTH_REDIRECT_URI=localhost3000
  - REACT_APP_SERVER=localhost3001
- last two go into netlify

- Functional Component
  - we don't need to worry about it
  - add bootstrap Button component

- Import buttons and profile into App
- Import Auth0 into App.js
- import { withAuth0 } from '@auth0/auth0-react';
- Wrap App
- export default withAuth0(App);

- Ternary
  - <>
    - in frag create ternary
  </>
- this.props.auth0.isAuthenticated
  - this asks if the user is logged in
  - ? : <LogoutButton/>
  - : : <LoginButton/>
  - this.props.auth0.isAuthenticated
  - ? <Profile/>
  - : : <h2>Please login</h2>

- Content.js
  - npm i axios
  - import React
  - import withAuth0 like above
  - export default content

  - class Content extends React.Component
  - render 
  - return
    - <h3>Content</h3>
  - constructor
    - setting state to books: []
  - event hadnler
    - getBooks = async () => {}
    - let url = `to server as template literal/books`
    - const bookResults = await axios.get(url);

- componentDidMount(){
  this.getBooks();
}
- We went to grab the const in our profile and paste it in in the render
- 

- Tokens
  - const res = await this.props.auth0.getIdTokenClaims();

- Must use double underscores!
  - const jwt = res.__raw;
  - console.log(jwt);
- get token to show up in terminal!

- const config = {
  method: 'get',
  baseUrl: process....
  url: '/books'
  headers: {"Authorization": `Bearer ${jwt}`}
}
const bookResults = await axios(config);

- ^^ this is for Auth0 and axios
- lab15 generate token

- backend
  - how to deal with json tokens
  - refer to demo code

- Jessica Parker
  - Alumni
  - negotiating offers
  - 40Au
  - made and founded by fevelopers for developers
  - web, mobile, data entry, robotics
  - happy, healthy, excited about job, fulfilled, sleep better, financially independent 
  - codefellows changed her life
  - wasn't the best in her class 
    - behind level of classmates
  - when you get to tough spots, remember your growth mindset
  - I am going to be least experienced and that's okay
  - being comfortable being uncomfortable
  - NETWORK NOW
    - delaying paycheck
    - planting a garden
    - post on linkedin
    - comment on posts
  - expectations for juniors are not super huge
  - Clean up LinkedIn!
  - Add old friends
  - network network network
  - Java is getting scooped up
  - Python could teach self
  - Python is #1 thing that her employer is looking for
  - Happy she did JS
  - learn lanuage deeply enough that you could teach yourself others
  - language was somewhat hindering on eomployment
  - she thinks you should know Javascript AND ..
  - commit to a bootcamp that says javascript and Python
  - negotiation
    - two competing offers in the same week as her partner
    - sounding board for each other
    - will company help you grow?
    - reach out to alumni network for negotiation advice
    - add on linkedIn
- When you graduate take a week off but build something to show that you have been active!! 
- always understand that if code breaks it's not you, your code and yourself are two different things. 
- its the CODE its NOT the PERSON

