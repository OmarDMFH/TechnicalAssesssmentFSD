
# ASP.NET Quiz

### **Scenario**: 
You are to develop a tiny ASP.NET 6 web application for "Dr. Mohammad Alfagih Hospital" to manage patient room assignments. This application should automate the process based on patients' treatment urgency, room availability, and specific medical needs.

**Requirements**:

- **Patients**: Each patient record should include a unique ID, a treatment urgency level (such as `emergency`, `high`, `standard`, `low`), and a list of medical needs (e.g., `oxygen`, `wheelchair access`).
- **Rooms**: Each room record should have a unique ID, a list of available medical equipment, and a status indicating whether it is currently occupied.
- The application must assign patients to rooms prioritizing treatment urgency and matching the patient's medical needs with the room's available equipment.
- If multiple rooms meet a patient's requirements, the system should assign them to the room with the lowest ID.
- The application should handle cases where no available room meets the patient's needs by indicating that no suitable room is available.

**Task**: Develop a tiny ASP.NET application that includes:

- A simple web form to input details for patients and available rooms.
- A backend method to process this input and assign patients to rooms based on the criteria mentioned.
- A results page that displays the assignment of patients to rooms.


**Sample Input** (for testing the application):

- Patients:
  - Patient 1: ID = 101, Urgency = `emergency`, Needs = [`oxygen`]
  - Patient 2: ID = 102, Urgency = `standard`, Needs = [`wheelchair access`]
- Rooms:
  - Room 1: ID = 1, Equipment = [`oxygen`, `wheelchair access`], Occupied = false
  - Room 2: ID = 2, Equipment = [`oxygen`], Occupied = false

**Expected Output** (displayed in the application view):

- Patient 101 is assigned to Room 1
- Patient 102 is assigned to Room 2

**Question**: Implement this web application using ASP.NET 6 or later version following the above specifications. Describe your approach to managing the data (e.g., in-memory collections, mock database).