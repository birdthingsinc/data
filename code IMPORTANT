# Simple databank system

database = {}  # Dictionary to store key-value pairs

def login():
    code = input("Enter your access code: ")
    if code == "th123":
        print("Access granted.")
        menu()
    else:
        print("Access denied. Incorrect code.")

def menu():
    while True:
        print("\n--- Data Bank Menu ---")
        print("1. Add Information")
        print("2. View Information")
        print("3. Delete Information")
        print("4. Exit")
        choice = input("Choose an option: ")

        if choice == "1":
            add_info()
        elif choice == "2":
            view_info()
        elif choice == "3":
            delete_info()
        elif choice == "4":
            print("Exiting the Data Bank. Goodbye!")
            break
        else:
            print("Invalid choice. Please try again.")

def add_info():
    key = input("Enter a key (name of data): ")
    value = input("Enter the information: ")
    database[key] = value
    print(f"Data saved: {key} -> {value}")

def view_info():
    if not database:
        print("No data found in the databank.")
    else:
        print("\n--- Stored Information ---")
        for key, value in database.items():
            print(f"{key}: {value}")

def delete_info():
    if not database:
        print("No data to delete.")
    else:
        key = input("Enter the key of the data to delete: ")
        if key in database:
            del database[key]
            print(f"Data under '{key}' deleted.")
        else:
            print(f"No data found with the key '{key}'.")

# Start the program
print("Welcome to the Data Bank System.")
login()
