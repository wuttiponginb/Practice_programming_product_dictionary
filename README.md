product = {}
count = 0
while count < 3:
    name_product = str(input("Enter product name: "))
    price_product = int(input("Enter product price: "))
    product[name_product] = price_product
    count += 1
print("---เพิ่มสินค้า---")
for key, value in product.items():
    print(f"ชิ่อสินค้า {key}")
    print(f"ราคา: {value}")

print("---รายการสินค้า---")
for key, value in product.items():
    print(f"่{key}: {value}")

print("---ค้นหาสินค้า---")
search = input("ค้นหา: ")
print(product.get(search, "ไม่พบสินค้า"))

print("---สรุป---")
print(f"แพงที่สุด: {max(product.keys())}: {max(product.values())}")
print(f"ถูกที่สุด: {min(product.keys())}: {min(product.values())}")
