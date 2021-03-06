## PHP Laravel - App for posting and viewing pictures

The App is made with PHP Artisan. The database is made using SQLite. The app will be extended in the future and more features will be added. The current features are:

- Login and Register users.
- Follow users and see their posts on the home page.
- Edit profile page and see your posts.
- Create posts. 

## How to Run

Make sure `PHP`, `nodeJS` and `composer` are installed, then navigate to the app directory. 

### Run the following when first staring the app:

`composer update`

`php artisan storage:link`

### Run this to start the app:

`php artisan serve`

The app will launch on `http://127.0.0.1:8000`. To interact with the database, use `php artisan tinker`.

### Some important routes:

`/` --> index homepage which shows the posts of the users followed by the logged in user. The logged user needs to follow other users to see the posts. Can be accessed by clicking on the logo. 

`/profile/{user}` --> the profile page for a `user` given a certain id, for example `/profile/1`. Use this route to access other profiles to follow them.
Use this route to navigate between users to follow/unfollow them and see their posts on the home page.

`/profile/{user}/edit` --> edits the profile of the given `user`.

`/p/{post}` --> shows an individual post given a post id.

`/p/create` --> creates a post and for the currently logged in user.

### Users already created which can be used to log in:

| Name | Email | Username | Password |
| ------------- | ------------- | ------------- | ------------- |
| John Doe | user1@yahoo.com | User1 | laravelapp1 |
| Jane Doe | user2@yahoo.com | User2 | laravelapp2 |
| Bob Rim | user3@yahoo.com | ThirdUser | laravelapp3 |
