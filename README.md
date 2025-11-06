# IDAI101-1000414-ADITYA-JITENDRA-KUMAR-SAHANI
**AI-Based Smart Solutions: Smart Campus Assistant**

[cite_start]**Course:** Artificial Intelligence: Real-World Applications and Implications [cite: 4]
[cite_start]**CRS:** Artificial Intelligence [cite: 4]
**Student:** Aditya Jitendra Kumar Sahani
**ID:** 1000414

---

## 1. 🔴 Live Chatbot Link

You can test the live, deployed chatbot here:

* **[PASTE YOUR WORKING LIVE CHATBOT URL HERE]**

---

## 2. Project Overview

This repository contains the "Smart Campus Assistant," a chatbot built using Google Dialogflow. It is a summative assessment project for the WACP course, "Artificial Intelligence: Real-World Applications and Implications."

[cite_start]The primary goal of this chatbot is to assist newcomers and regular campus users (like students, parents, staff, and visitors) by providing quick answers about department locations, event venues, office hours, campus policies, transportation options, and emergency contacts[cite: 6]. [cite_start]This AI assistant serves as a reliable, accessible guide to enhance the campus experience for all[cite: 6].

### Target Users

[cite_start]The primary users for this chatbot include[cite: 39]:
* New Students
* Guests
* Parents
* Staff and existing students

---

## 3. List of Intents & Entities

[cite_start]This chatbot was implemented with **15 intents** and **10 custom entities** to handle a wide range of user queries, as required by the project brief[cite: 6].

### Intents

Here is a list of the 15 intents built for this agent:

| Intent Name | Description | Example User Queries |
| :--- | :--- | :--- |
| `Default Welcome Intent` | Greets the user and starts the conversation. | "Hi", "Hello", "Good morning" |
| `Default Fallback Intent`| Catches any queries the chatbot doesn't understand. | (Handled by Dialogflow) |
| `find_academic_building`| Provides the location of a specific academic building. | [cite_start]"Where is the Science Block?", "Find the Engineering Hall" [cite: 47] |
| `find_event` | Finds the location or time for a campus event. | [cite_start]"Where's today's seminar happening?", "What's on this weekend?" [cite: 47] |
| `find_hours` | Provides the operating hours for a campus service or facility. | [cite_start]"What are the library hours?", "When does the admin office open?" [cite: 47] |
| `find_lab` | Gives directions to a specific computer or science lab. | [cite_start]"I need directions to the Computer Science lab", "Where is the physics lab?" [cite: 47] |
| `find_location` | A general intent to find non-academic locations. | "Where is the cafeteria?", "Find the nearest restroom" |
| `find_professor_office` | Locates the office of a specific professor. | "Where is Professor Sharma's office?", "Find Dr. Singh" |
| `find_service_building` | Locates a specific student or campus service building. | [cite_start]"Where is the admin office?", "How to get to the library?" [cite: 40] |
| `get_contact` | Provides contact details (phone/email) for a department. | "How do I contact the admin office?", "What's the library's phone number?" |
| `get_emergency_contact`| Provides critical emergency contact information. | [cite_start]"I need help", "Emergency on campus", "Campus security number" [cite: 6] |
| `get_nearby_recreation` | Recommends nearby recreational activities or places. | [cite_start]"What is there to do around here?", "Nearby parks or cafes" [cite: 6] |
| `get_policy` | Explains a specific campus policy or rule. | [cite_start]"What is the attendance policy?", "Tell me the hostel rules" [cite: 6] |
| `get_transportation` | Gives information on transportation options. | [cite_start]"Campus bus schedule", "Where is the nearest metro?" [cite: 6] |
| `Goodbye` | Ends the conversation. | "Thanks, bye", "See you later", "That's all" |

### Entities

Here is a list of the 10 custom entities created to extract data:

| Entity Name | Description | Examples |
| :--- | :--- | :--- |
| `@academic_building` | Captures the names of academic buildings. | "Science Block", "Engineering Hall", "Arts Building" |
| `@contact_type` | Captures the type of contact info requested. | "Phone", "Email", "Address" |
| `@event_name` | Captures the specific name of a campus event. | "Seminar", "Workshop", "Tech Fest" |
| `@facility` | Captures general campus facilities. | "Gym", "Cafeteria", "Student Lounge" |
| `@lab_name` | Captures the names of specific labs. | "Computer Science lab", "Physics lab", "Chem lab" |
| `@location` | Captures general locations (non-academic). | "Main gate", "Restroom", "ATM" |
| `@policy_type` | Captures the type of campus policy. | "Attendance", "Hostel", "Exam", "Library" |
| `@professor_name` | Captures the names of professors. | "Professor Sharma", "Dr. Singh" |
| `@recreation_type` | Captures types of recreational activities. | "Park", "Cafe", "Gym", "Shopping" |
| `@service_building` | Captures the names of service buildings. | "Library", "Admin Office", "Admissions", "Hostel" |

---

## 4. Integration Details

* **Platform:** The chatbot is built and hosted on **Google Dialogflow Essentials**.
* [cite_start]**Slot-Filling:** Slot-filling is used in intents like `find_professor_office` to collect all necessary information (e.g., the `@professor_name`) before providing a complete answer[cite: 47].
* [cite_start]**Rich Responses:** The chatbot uses rich responses to enhance user engagement[cite: 47], including:
    * **Suggestion Chips:** Used for navigation options (e.g., "View Map", "Get Directions") or to suggest follow-up queries.
    * [cite_start]**Media Responses:** Used to display images like campus maps or event banners to provide clearer, more helpful answers[cite: 47].

---

## 5. Deployment Instructions

[cite_start]The chatbot is already deployed and accessible via the live link in Section 1[cite: 47].

To import this agent into your own Google Dialogflow project:
1.  Download the `agent.zip` file (if included in this repository).
2.  Go to the Google Dialogflow ES console and create a new agent.
3.  Click the **Gear Icon** (⚙️) to open Agent Settings.
4.  Go to the **Export and Import** tab.
5.  Select **Import from Zip** and upload the `agent.zip` file.
