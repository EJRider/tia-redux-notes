# Weekend Challenge 11 - React-Redux Feedback Form

## Instructions

Reviewing code is an important role developers play. We're going to practice reviewing code from others.

- Get the repo url from your partner
- Get your partner's project running on your computer
- Review the code from your partner and give relevant feedback
- Complete the Markdown section and submit that in the notes section on the assignment app. (Make sure you include who's code you reviewed.)

Practicing compassionate code reviews is important (you can learn more from this video on the topic: https://www.youtube.com/watch?v=Ea8EiIPZvh0 )

## Review Checklist

## Base Required Features 

- Multi-Part Form:  
  - [x] Able to add feedback
    - [x] Data collected on individual pages & components
    - [x] Click on next takes you to the next page in sequence
    - [x] Data saves in DB after *all* the parts are completed (not piecemeal)
    - [x] Thank you page takes you back to the first view
    - [x] Old Data is cleared on form completion

- Client code:
  - [x]  Individual components for each form part
  - [x]  Redux setup complete
    - [x] Store linked to react with `<Provider>`
    - [x] Store setup with reducer(s) and logger middleware 
  - [x] Reducers & Actions Working
    - [x] Actions are in SCREAMING_SNAKE_CASE and semantically named
    - [x] Actions have a `type` key, and `payload` if sending data
    - [x] Reducers are returning a new state, or the old state (not mutating)
    - [x] Reducers are using spread correctly (to keep old data, while adding new)
  - [x] Review Component shows at all times with current redux state
  - [x] React-Redux Working
    - [x] Dispatching actions onClick
    - [x] Grabbing data from the redux store with `useSelector`
  - [x] Axios POST request to add feedback


- Server code:   
  - [x] Router made for GET, POST


## General Items
Feedback should be provided for these items, but they do not impact scoring.

- Git 
  - [x] Multiple git commits showing incremental progress
  - [x] Commits are descriptive of the changes made or feature added 
  - [x] Has .gitignore with node_modules
  - [ ] Readme file updated (assuming this is previously discussed)
- Code Style 
  - [x] Appropriate amount of code comments
  - [x] Code is consistently formatted
- Client
  - [x] Appropriate use of HTML tags
  - [x] Basic CSS styling with margins/padding


## Stretch Goals
First must be complete for score of  _Exceeds Expectations_

- Previous Steps
  - [ ] allows a user to go to a previous step, either directly or by cycling backward thru the steps
  - [ ] user can upate their score for a step
    - [ ] new score is validated to not be empty
    - [ ] redux is updated with new score
  - [ ] user can continue on to review page and submit as in Base Mode


- Admin View
  - [ ] All entries are visible with correct data from inputs
    - [ ] Most recent is at the top
  - [ ] Can Delete an entry
    - [ ] User is prompted before deleting
  - [ ] Axios GET request to get all feedback for `/admin` view in componentDidMount

  Busywork Goals, consider removing or making more useful

- [ ] Styling with Material UI
- [ ] Ability to flag a feedback item on `/admin` for further review
- [ ] Deployed to Heroku


## Markdown

```
Hey ___,

General Feedback.

---
| Functional Requirements | Complete? |
| --- | :---: |
| Multi page form with client side routing and navigation (next button) | Yes |
| Data stored in Redux when navigating from page to page | Yes |
| User is notified when trying to leave a blank score | Yes |
| Review Component displays scores and comments from current redux state | Yes |
| Submit button sends data to the server via Axios | Yes |
| Confirmaion Page displays after data is POSTed to the server | Yes |
| Button on Confirmation Page clears Redux and starts a new survey | yes |
| Views are broken down into components | Yes |

---
### Notes:

This looks great! I can clearly tell what each line of code is doing! Awesome use of passing functions and data into the different components! If you want you can also use that useSelector inside a component the same way (Might save a bit of typing). Great job with the min and max for your inputs! I didn't think to do that myself but it makes the program a bit more protected from user mistakes. 

---
| General Items | Complete? |
| --- | :---: |
| More than 15 git commits | Yes |
| Commits are descriptive of the changes made or feature added | Yes |
| Readme file updated | no |
| Appropriate amount of code comments | Yes |
| Code is consistently formatted | Yes |
| Server code organized with router & module files | Yes |

---
### Notes:

Great commits and code comments! Made it super easy to understand what your code was doing and where stuff was going! I would have love to have read a README, as would future users are aren't quite tech savvy as I am. Overall a great job though and I can't wait to see what you make in the coming weeks!
