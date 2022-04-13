# Create the database shown in the ER diagram below in Python and insert one example

## Python Code
```.py
import sqlite3
class electric_data(): # Class to create the database
    def __init__(self,db_name):
        self.name=db_name
        self.connection=sqlite3.connect(self.name)
        self.cursor=self.connection.cursor()

    def create(self): # This will create the table in the database
        self.cursor.execute("""create table if not exists electric_cars 
        (id integer primary key, # Create row called "key"
        brand varchar (255), # Create row called "brand"
        model varchar (255), # Create row called "model"
        maker varchar (255), # Create row called "maker"
        battery_size integer);""") # Create row called "battery_size"
        self.connection.commit()

    def add_car(self): # This class creates and adds a car in the database
        self.cursor.execute("""
        INSERT INTO Electric_cars (id, brand, model, maker, battery_size) values (1, "Tesla", "Model 3", "Tesla", 90000);
        """)
        self.connection.commit()
        
db=electric_data("quiz39.db")
# These execute the commands
db.create()
db.add_car()
```

## Output:

![](quiz39.png)
