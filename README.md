# shopping-cart-program
foods = []
prices = []
total = 0

while True:
    food = input("enter the food(q to exit)-")
    if food.lower() == "q":
        break
    else:
        price = float(input(f"enter the price of the {food} - "))
        foods.append(food)
        prices.append(price)
        
print("-----Your Cart-----")

for food in foods:
    print(food , end=" ")
    
for price in prices:
    total += price
    
    print(f"your final price of {food} is {total}")
