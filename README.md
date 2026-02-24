# Grocery-Billing-System_Mohammad-Saadman-Kha_202501100700199_B

total = 0

for i in range(1, 6):
    print(f"\nItem {i}")
    
    price = float(input("Enter price: "))
    units = int(input("Enter number of units: "))
    
    item_total = price * units
    total += item_total

original_total = total
discount = 0

if total > 100:
    discount = total * 0.10
    total = total - discount

print("\n------ BILL DETAILS ------")
print("Original Total: Rs.", original_total)
print("Discount: Rs.", discount)
print("Final Amount to Pay: Rs.", total)
