//create new project
django-admin startproject projectname

//install rest framework
pip install djangorestframework

//run the application local
python manage.py runserver

// create new app inside project
python manage.py startapp projectname

//migrate the created model
python manage.py makemigrations

//apply the migrations
python manage.py migrate

//shell command to start working with data
python manage.py shell

from base.models import Item //(base=projectname) and (model = model.py type inside the project base) importing the class "Item"
Item.objects.create(name="item #1") //insert data object
Item.objects.create(name="item #1") //insert data object

items = Item.objects.all() //save the data created
print(items) //print to terminal

exit() //exit the terminal of py shell
