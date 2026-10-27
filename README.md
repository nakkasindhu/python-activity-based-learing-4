# python-activity-based-learing-4
Algorithm
1.Start.
2.Enter raw materials, production quantity, defects, and order demand.
3.Check material availability.
4.Calculate shortages and good products.
5.Check quality violations.
6.Display results and stop.
flowchart
Start
Input production details
Check materials and demand
Calculate shortages and defects
Display results
Stop
material = int(input("Available materials: "))
production = int(input("Production quantity: "))
demand = int(input("Order demand: "))
defects = int(input("Defective products: "))

if material < production:
    print("Material shortage:", production - material)
else:
    print("Materials sufficient")

good = production - defects
print("Good products:", good)

if good < demand:
    print("Order shortage:", demand - good)
else:
    print("Order satisfied")

if defects > production * 0.05:
    print("Quality violation")
    Available materials: 100
Production quantity: 120
Order demand: 110
Defective products: 10

Material shortage: 20
Good products: 110
Order satisfied
Quality violation
