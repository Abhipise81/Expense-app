# Expense-app

An expense management react application to compliment with the [expense-api](https://github.com/Abhipise81/Expense-api)  backend.

All the information related to app is provided in this file

# Features Completed
  - [x] Sign up
  - [x] Login
  - [x] Logout
  - [x] Update Total Budget
  - [x] Create Category
  - [x] List Category
  - [x] Delete Category
  - [x] Restore Category
  - [x] Create Expense
  - [x] Edit Expense
  - [x] List Expense (With pagination 10 entry per page)
  - [x] Delete Expense
  - [x] Restore Expense
  - [x] Update Name
  - [x] Update Username
  - [x] Change Password

## Sign up, Login and Logout

1. Signup application is provided for new user on login page.
2. there are four fields name, username, password and confirm password (total budget will be provided by user on first login).
3. Every field in signup form has field validation
    - all fields must me filled
    - username, password should be at least 6 character long
    - confirm password should match password
4. After successful Signup a success screen will be shown and a option for go to login is provided for easy navigation.
5. After Clicking on go to login user is redirected to login.
6. There are three field in Login form Username, password, remember me.
7. If user selects remember me option his session will be available for all the tabs in current browser untill the token is expired if user does not come back to the application for three consecutive days user's session token will be expired and user will be logged out.
8. if user does not select remember me user session will be valid for that tab only after user closes tab or browser user will be logged out.
9. after validating the username & password user is logged in and depending on the total budget key he will be redirected to home (If total budget is set) or settings(If total budget is not set).
10. **Logout** option is provided in sidebar

## Settings (Total budget update & Category Create, Read, Delete)

1. User can update his total budget and create categories on this page
2. User can delete particular category by clicking delete button provided in actions column
3. User can find the activation status of category in status column, background color of row and red color of row text
4. user can restore the category by clicking restore button

## Home (Expense CRUD, Budget overview, Category wise split)

1. In first row I added two charts one is doughnut chart and other is pie chart which givers the info about how much money is spent how much percent is spent and category wise spending
2. if there are more than five categories table will be shown instead as shown in below screenshot
3. Add expenses button is provided in second row a modal with form will be shown
4. expense has four fields category dropdown, Item name, Amount, Data
5. after creating the expense it will be updated in the expense table below the button
6. In expense table Edit option is provided for every entry when edit button is pressed update expense form on modal will be shown with prepopulated values this form is the same as add expense from both forms are shown below

#### Update Expense Modal

7. Delete option is provided in action column for every entry if delete is pressed a action confirmation modal like below will popup for confirmation this will happen  for restore to this is same functionality like delete and restore category

#### Confirmation Modal

8. After deleting expense that row will become red and status will become inactive to show user that this entry is deleted
user can restore the entry using restore button

## Profile (Update Name, Username, Change Password)

1. On profile page update Name ,Update Username and Change password is provided
2. field validation are added for all these fields

Technologies/Libraries Used
--------------

1. JavaScript
2. React Js (React hooks, react-router-dom, react-dom)
3. Bootstrap (react-bootstrap)
4. chart.js
5. styled-components
6. react-toastify
7. axios

Instructions
--------------
Please follow these instructions for running the application.

###### APP
- [] Install nodejs, npm ,yan on your machne
- [] clone expense-app repo
- [] install all the dependencies using ```yarn```
- [] start server using ```yarn start```


- there is warning for ./local module not found after starting the server ignore this warning as this is related to chart.js and it will be resolved in their next update
