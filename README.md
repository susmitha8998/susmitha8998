def calculate_salary():
    employee=[]
    while True:
        employee_name=input("enter employee name(type'exit' to stop):")
        if employee_name=="exit":
            break
    try:
           hours_worked=float(input("enter hours worked:"))
           hourly_rate=float(input("enter hourly rate:"))
    except ValueError:
           print("invalid input!please enter valid numbers")
           Continue
    if hours_worked<0 or hourly_rate<0:
           print("hours worked and hourly rate cannot be negative")
           Continue
           salary=hours_worked*hourly_rate
           employee.append(employee_name.salary)
           return employee
if __name__=="__main__":
 print("welcome to employee salary calculator")
 employee_data=calculate_salary()
 print("\n employee salary details:")
 for name,salary in employee_data:     
     print(f"{name}:${salary:.2f}")

