### Django API (Ribbit)

A backend only Django Project which allows users to Make Posts and Vote for them, made using the REST API framework.
Just a beginner Clone project, to familiarize with the concepts of a Python API. All the Data are Viewed as JSON files which are obtained after a GET request to the REST Framework.

### Run the code
``` 
python manage.py makemigrations
python manage.py migrate

python manage.py runserver
```
### URLS
 
This project contains a few specific URLS which all have certain tasks. the project Urls can be obtained as an extension to the (localhost) ```http://127.0.0.1:8000/```. The URLS are as follows:-
1) ```api/posts``` : Views all the posts that have been made along with the user who made the post along with the number of votes it has. The JSON file displays the newest post first.
2) ```api/posts/<int:pk>``` : Shows a particular post indicated by a unique key. allows the user to modify and even delete the post once authenticated.
3) ```api/posts<int:pk>/vote``` : Views the Votes of a certain post indicated by its unique key. Allows the User to cast their vote only once on a particular post.
4) ```api-auth/``` : Checks if the User is authenticated. If a User isn't authenticated they wont be able to make posts or Vote a=or alter the status of an existing Post or vote.
5) ```admin``` : Allows the Admin to access the SQLite Database after logging in using the correct credentials.

### Install the following

Install Django3 or the latest version by running 
```
pip install Django
```
Install using ```pip```, including any optional packages you want...

```
pip install djangorestframework
pip install markdown       # Markdown support for the browsable API.
pip install django-filter  # Filtering support
```
...or clone the project from github.

```
git clone https://github.com/encode/django-rest-framework
```
