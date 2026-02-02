# IMPLEMENTING-MODULES-CLASSES-AND-INSTANCES
def add(a, b):
return a + b
def sub(a, b):
return a - b
import math_module
print(math_module.add(10, 5))
print(math_module.sub(10, 5))
class Student:
def __init__(self, name, marks):
self.name = name
self.marks = marks
def display(self):
print(self.name, self.marks)
s1 = Student(&quot;Ravi&quot;, 85)
s2 = Student(&quot;Anita&quot;, 92)

s1.display()
s2.display()

Output:
15
5
Ravi 85
Anita 92
7. EXERCISE BY ILLUSTRATING REGULAR EXPRESSION
import re
phone = input(&quot;Enter your phone number (format XXX-XXX-XXXX): &quot;)
phone_pattern = r&quot;^\d{3}-\d{3}-\d{4}$&quot;
if re.match(phone_pattern, phone):
print(&quot;Phone number is valid!&quot;)
else:
print(&quot; Invalid phone number format!&quot;)

password = input(&quot;Enter your password: &quot;)
password_pattern = r&quot;^(?=.*[a-z])(?=.*[A-Z])(?=.*\d).{8,}$&quot;
if re.match(password_pattern, password):
print(&quot;Strong password!&quot;)
else:
print(&quot;Weak password! Make sure it has at least 8 characters, including:&quot;)
print(&quot; - 1 uppercase letter&quot;)
print(&quot; - 1 lowercase letter&quot;)
print(&quot; - 1 digit&quot;)
Output:
Enter your phone number (format XXX-XXX-XXXX): 999-985-9234
Phone number is valid!
Enter your password: psgr@123
Weak password! Make sure it has at least 8 characters, including:
- 1 uppercase letter
- 1 lowercase letter
- 1 digit
