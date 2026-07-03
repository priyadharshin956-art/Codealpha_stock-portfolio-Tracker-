stocks = {
    "AAPL": 180,
    "TSLA": 250,
    "GOOGL": 150,
    "MSFT": 300
}

total = 0

n = int(input("Enter number of stocks: "))

for i in range(n):
    stock = input("Enter stock name: ").upper()
    quantity = int(input("Enter quantity: "))

  if stock in stocks:
      total += stocks[stock] * quantity
   else:
        print("Stock not found!")

print("\nTotal Investment Value = $", total)
