# Flask-Migrate

**First, Installing Flask-Migrate**

``` $ pip3 install Flask-Migrate```


**Then Importing the Migrate library and creating an instance of the Migrate class**

```
from flask_migrate import Migrate

db = SQLAlchemy(app)
migrate = Migrate(app, db)
```


**Creating the migrations directory structure**

```$ python3 -m flask db init```


**Detects the model changes to be made, and create a migration file with upgrade and downgrade logic set up.**
**(replace use of db.create_all())**

```$ python3 -m flask db migrate -m "Initial migration."```

**Run the upgrade command in migration file, to apply the migration**

```$ python3 -m flask db upgrade```


**Run the downgrade command in migration file, to roll back the migration**

```flask db downgrade```


Resource: 
- https://flask-migrate.readthedocs.io/en/latest/
- https://alembic.sqlalchemy.org/en/latest/
