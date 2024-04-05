# WOMEN SAFETY IN TRAINS (Expert System)

* An expert system for women's safety in railway stations can provide several benefits in addressing the unique challenges and concerns faced by women in these public spaces. Here are some reasons why such an expert system could be valuable:
1.Tailored Guidance
2.Real-Time Assistance
3.Information Dissemination
4.Risk Assessment
5.Integration with Surveillance Systems
6.Emergency Response Coordination

*Problem Solution(Code):
class WomenSafetySystem:
    def __init__(self):
        self.helpline_numbers = {
            "Police": "100",
            "Women's Helpline": "1091",
            "Railway Protection Force (RPF)": "182",
        }

    def display_helpline_numbers(self):
        print("Emergency Helpline Numbers:")
        for service, number in self.helpline_numbers.items():
            print(f"{service}: {number}")
    
    def send_alert(self, location):
        alert_message = f"Emergency: Woman in distress at {location}. Please take immediate action!"
        print(alert_message)
        # In a real-world scenario, you might send alerts through SMS, push notifications, or other means.
    
    def report_incident(self, location):
        # In a real-world scenario, you might report incidents to the authorities.
        print(f"Incident reported at {location}. Authorities notified.")

    def main(self):
        print("Welcome to the Women's Safety System for Trains!")

        while True:
            print("\nOptions:")
            print("1. Display Helpline Numbers")
            print("2. Send Emergency Alert")
            print("3. Report Incident")
            print("4. Exit")

            choice = input("Enter your choice (1-4): ")

            if choice == "1":
                self.display_helpline_numbers()
            elif choice == "2":
                location = input("Enter your current location: ")
                self.send_alert(location)
            elif choice == "3":
                location = input("Enter incident location: ")
                self.report_incident(location)
            elif choice == "4":
                print("Exiting Women's Safety System. Stay safe!")
                break
            else:
                print("Invalid choice. Please enter a number between 1 and 4.")

if __name__ == "__main__":
    safety_system = WomenSafetySystem()
    safety_system.main()

*OUTPUT:
Welcome to the Women's Safety System for Trains!

Options:
1. Display Helpline Numbers
2. Send Emergency Alert
3. Report Incident
4. Exit
Enter your choice (1-4): 1
Emergency Helpline Numbers:
Police: 100
Women's Helpline: 1091
Railway Protection Force (RPF): 182

Options:
1. Display Helpline Numbers
2. Send Emergency Alert
3. Report Incident
4. Exit
Enter your choice (1-4): 2
Enter your current location: xyz
Emergency: Woman in distress at xyz. Please take immediate action!

Options:
1. Display Helpline Numbers
2. Send Emergency Alert
3. Report Incident
4. Exit
Enter your choice (1-4): 3
Enter incident location: xyz
Incident reported at xyz. Authorities notified.

Options:
1. Display Helpline Numbers
2. Send Emergency Alert
3. Report Incident
4. Exit
Enter your choice (1-4): 4
Exiting Women's Safety System. Stay safe!









