```.py
class Employee:
    # This is a class for the HR department
    def __init__(self, name:str, email:str, age:int, salary:int, position:str):
        self.name=name
        self.email=email
        self.age=age
        self.salary=salary
        self.position=position

    def getgreeting(self):
        out = f"Hello {self.name.title()}, you are {self.age} years old and work as a {self.position} in our company. " \
              f"Your email address is {self.email}"
        return out
    def __repr__(self):
        out = f"<Class Employee> Hello {self.name.title()}, you are {self.age} years old and work as a {self.position} in our company. " \
              f"Your email address is {self.email}"
        return out

    def getsalary (self)->str:
        return f"Salary for {self.name.title()} is {self.salary}USD"

    def set_salary(self,new_value:int):
        # This function updates the salary of the selected employee
        self.salary = new_value
    def set_name(self,new_name:str):
        self.name=new_name
    def getname(self)->str:
        return f"Your name is {self.name}"
    def set_age(self,new_age):
        self.age=new_age
    def getage(self)->str:
        return f"Your age is {self.age}"
Emp_1 = Employee(name="frankmurphy", email="frank.murphy@company.xy", position="driver", age=39, salary=30000)
Emp_10 = Employee(name="VitoCorleone", email="vitocorleone@company.xy", position="mafia", age=65, salary=30000000)
Emp_3 = Employee(name="Bezos", email="bezos@company.xy", position="clown", age=85, salary=1000)


print(Emp_1.getgreeting())
print(Emp_10.getgreeting())
print(Emp_3.getgreeting())
print(Emp_1)
print(Emp_1.getsalary())
Emp_1.set_salary(-999999)
print(Emp_1.getsalary())
Emp_1.set_name("Bobby")
print(Emp_1.getname())
Emp_1.set_age(8934)
print(Emp_1.getage())
```
