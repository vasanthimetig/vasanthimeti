from datetime import datetime

class Admin:
    def __init__(self, name, phone, email):
        self.name = name
        self.phone = phone
        self.email = email

class Doctor(Admin):
    def __init__(self, name, phone, email):
         self.name = name
         self.phone = phone
         self.email = email
         self.appointments = []
    
    def availability(self, appointment_time):
        for appointment in self.appointments:
            if appointment == appointment_time:
                return "Doctor unavailable"
        return "Doctor is Available"

    def send_reminder(self, appointment):
        print(f"Reminder sent to Dr. {self.name} for appointment on {appointment.strftime('%Y-%m-%d %H:%M')}.")

class Patient(Admin):
    def _init_(self, name, phone, email):
         self.name = name
         self.phone = phone
         self.email = email

    def send_reminder(self, appointment):
        print(f"Reminder sent to {self.name} for appointment on {appointment.strftime('%Y-%m-%d %H:%M')}.")

appointment = input("Enter appointment date (YYYY-MM-DD HH:MM): ")
appointment_datetime = datetime.strptime(appointment, "%Y-%m-%d %H:%M")

doctor = Doctor("Dr. XYZ", "123-456-7890", "dr.xyz@example.com")
patients = []

while True:
    name = input("Enter patient name (leave empty to finish): ")
    if not name:
        break
    phone = input("Enter patient phone number: ")
    email = input("Enter patient email: ")
    
    patient = Patient(name, phone, email)
    patients.append(patient)

def display(doctor, patients, appointment):
    print("APPOINTMENT DETAILS:\n")
    print("Doctor Details:")
    print(f"Doctor name: {doctor.name}\nPhone number: {doctor.phone}\nEmail: {doctor.email}")
    print(f"\nSCHEDULED PATIENTS FOR - {appointment.strftime('%Y-%m-%d %H:%M')}\n")
    for patient in patients:
        print(f"Patient name: {patient.name}\nPhone number: {patient.phone}\nEmail: {patient.email}\n")

current_time = datetime.now()
print(f"CURRENT TIME: {current_time}")
print(f"\nSELECTED APPOINTMENT DATE: {appointment}\n")
print(doctor.availability(appointment_datetime), "\n")
display(doctor, patients, appointment_datetime)

while True:
    print("\nSelect an option:\n1. Confirm appointments\n2. Delete appointment\n3. Send reminders\n\n4.EXIT\n")
    option = int(input())
    if option == 1:
        doctor.appointments.append(appointment_datetime)  
        print("\nAPPOINTMENTS CONFIRMED\n")
        for patient in patients:
            print(f"Appointment added for {patient.name} with {doctor.name} at {appointment_datetime}\n")
    elif option == 2:
        if appointment_datetime in doctor.appointments:
            doctor.appointments.remove(appointment_datetime)  
            print("\nAPPOINTMENT DELETED \n")
    elif option == 3:
         for patient in patients:
            patient.send_reminder(appointment_datetime)
         doctor.send_reminder(appointment_datetime)
    elif option==4:
        print("\n EXIT")
        break
from datetime import datetime

class Admin:
    def __init__(self, name, phone, email):
        self.name = name
        self.phone = phone
        self.email = email

class Doctor(Admin):
    def __init__(self, name, phone, email):
         self.name = name
         self.phone = phone
         self.email = email
         self.appointments = []
    
    def availability(self, appointment_time):
        for appointment in self.appointments:
            if appointment == appointment_time:
                return "Doctor unavailable"
        return "Doctor is Available"

    def send_reminder(self, appointment):
        print(f"Reminder sent to Dr. {self.name} for appointment on {appointment.strftime('%Y-%m-%d %H:%M')}.")

class Patient(Admin):
    def _init_(self, name, phone, email):
         self.name = name
         self.phone = phone
         self.email = email

    def send_reminder(self, appointment):
        print(f"Reminder sent to {self.name} for appointment on {appointment.strftime('%Y-%m-%d %H:%M')}.")

appointment = input("Enter appointment date (YYYY-MM-DD HH:MM): ")
appointment_datetime = datetime.strptime(appointment, "%Y-%m-%d %H:%M")

doctor = Doctor("Dr. XYZ", "123-456-7890", "dr.xyz@example.com")
patients = []

while True:
    name = input("Enter patient name (leave empty to finish): ")
    if not name:
        break
    phone = input("Enter patient phone number: ")
    email = input("Enter patient email: ")
    
    patient = Patient(name, phone, email)
    patients.append(patient)

def display(doctor, patients, appointment):
    print("APPOINTMENT DETAILS:\n")
    print("Doctor Details:")
    print(f"Doctor name: {doctor.name}\nPhone number: {doctor.phone}\nEmail: {doctor.email}")
    print(f"\nSCHEDULED PATIENTS FOR - {appointment.strftime('%Y-%m-%d %H:%M')}\n")
    for patient in patients:
        print(f"Patient name: {patient.name}\nPhone number: {patient.phone}\nEmail: {patient.email}\n")

current_time = datetime.now()
print(f"CURRENT TIME: {current_time}")
print(f"\nSELECTED APPOINTMENT DATE: {appointment}\n")
print(doctor.availability(appointment_datetime), "\n")
display(doctor, patients, appointment_datetime)

while True:
    print("\nSelect an option:\n1. Confirm appointments\n2. Delete appointment\n3. Send reminders\n\n4.EXIT\n")
    option = int(input())
    if option == 1:
        doctor.appointments.append(appointment_datetime)  
        print("\nAPPOINTMENTS CONFIRMED\n")
        for patient in patients:
            print(f"Appointment added for {patient.name} with {doctor.name} at {appointment_datetime}\n")
    elif option == 2:
        if appointment_datetime in doctor.appointments:
            doctor.appointments.remove(appointment_datetime)  
            print("\nAPPOINTMENT DELETED \n")
    elif option == 3:
         for patient in patients:
            patient.send_reminder(appointment_datetime)
         doctor.send_reminder(appointment_datetime)
    elif option==4:
        print("\n EXIT")
        break
