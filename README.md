# People Counter - Python Project
# Developed by: aishwaryapujari

count = 0

def people_counter():
    global count
    print("=== Smart People Counter ===")
    while True:
        action = input("Enter 'in' / 'out' / 'q': ").lower()
        if action == 'in':
            count += 1
            print(f"Person IN -> Total inside: {count}")
        elif action == 'out':
            count -= 1
            if count < 0:
                count = 0
            print(f"Person OUT -> Total inside: {count}")
        elif action == 'q':
            break
        else:
            print("Invalid input")
    print(f"Final count: {count}")

if __name__ == "__main__":
    people_counter()# people--counter
