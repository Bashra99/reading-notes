# Django Custom User Model

Django ships with a built-in User model for authentication, however the official Django documentation highly recommends using a custom user model for new projects. 
The reason is if you want to make any changes to the User model down the road.
for example adding a date of birth field--using a custom user model from the beginning makes this quite easy. But if you do not, 
updating the default User model in an existing Django project is very, very challenging.


So always use a custom user model for all new Django projects. 
However the official documentation example is not actually what many Django experts recommend using. 
There is a far easier yet still powerful approach to starting off new Django projects with a custom user model which I'll demonstrate here.

## Setup
To start, create a new Django project from the command line. We need to do several things:

  - create and navigate into a dedicated directory called accounts for our code
  - install Django
  - make a new Django project called config
  - make a new app accounts
  - start the local web server
  




## AbstractUser vs AbstractBaseUser
There are two modern ways to create a custom user model in Django: AbstractUser and AbstractBaseUser.
In both cases we can subclass them to extend existing functionality however AbstractBaseUser requires much, much more work. 

So we'll use AbstractUser which actually subclasses AbstractBaseUser but provides more default configuration.

### Custom User Model
Creating our initial custom user model requires four steps:

- update config/settings.py
- create a new CustomUser model
- create new UserCreation and UserChangeForm
- update the admin




