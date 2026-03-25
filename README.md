# Train-ticket-booking
# Ticket Booking System
# Name: Sudheksha P
# Department: CCE

print("🎟️ Welcome to Ticket Booking System")

# Available tickets
total_tickets = 50

while True:
    print("\nAvailable Tickets:", total_tickets)
    
    name = input("Enter your name: ")
    tickets = int(input("Enter number of tickets to book: "))
    
    if tickets <= 0:
        print("❌ Please enter a valid number of tickets.")
    
    elif tickets > total_tickets:
        print("❌ Not enough tickets available.")
    
    else:
        total_tickets -= tickets
        print("✅ Booking Successful!")
        print("Name:", name)
        print("Tickets Booked:", tickets)
        print("Remaining Tickets:", total_tickets)
    
    choice = input("\nDo you want to book again? (yes/no): ").lower()
    
    if choice != "yes":
        print("🙏 Thank you for using Ticket Booking System!")
        break
