# Cours Openclassroom Django Disquaire

https://openclassrooms.com/fr/courses/4425076-decouvrez-le-framework-django?status=published

Quelques notes : 

## ENV Virtuel 

Création : 

> virtualenv -p python3 env

Activation : 

> source env/bin/activate

Figer la config : 

> pip freeze > requirements.txt

Installer suivant le fichier 

> pip install -r requirements.txt

Desactiver l'ENV virtuel : 

> deactivate

Autres : 

>

> which python

> rm -rf env

>

## Git 

git ignore : 

Rajouter le dossier env/

## Migration 

> 
> ./manage.py makemigrations
>
> ./manage.py migrate
>
> ./manage.py showmigrations
>

## psql

>
> psql bdd
>
> \l        # Liste des  
>
> \dt       #liste des tables 
>
> \d table
>

## Console django 


>
> ./manage.py shell
>
> from store.models import Artist, Album
>
>  patrick = Artist(name="Patrick Bruel")
>
> patrick.save()
>
> francis = Artist.objects.create(name="Francis Cabrel")
>
> album = Album.objects.create(title="Sarbacane")
>
> album.artists.add(francis)
>
> Artist.objects.all()
>
> Artist.objects.filter(name="Francis Cabrel")
>
>
>
>