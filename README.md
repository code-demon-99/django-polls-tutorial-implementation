# done 
Completed the django tutorial for creating a polls app as per Django documentation 

the project has two parts 
- the main django project 
- a standalone polls app which can be installed on the main project and used properly  

using app
1.  python -m pip install pipenv
1. pipenv install 
1. pipenv shell 
1. python -m pip install  polls/dist/django-polls-0.1.tar.gz
1. cd mysite
1. python manage.py runserver
____ 
1.  if you want to use the polls app to separate project just copy polls/dist/django-polls-0.1.tar.gz and install as done above  and include in installed apps like below 

    INSTALLED_APPS = [
        ...
        'polls',
    ]
1. and add this to your urls.py as suggested

  path('polls/', include('polls.urls')),

1. now run python manage.py migrate 


and hence you can run this app anywhere on supported django version  mine was 4.1


