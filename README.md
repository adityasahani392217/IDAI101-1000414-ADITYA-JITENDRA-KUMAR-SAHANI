# Smart Campus Assistant
### AI-Based Conversational Guide for Campus Navigation & Support

**Course:** Artificial Intelligence – Real-World Applications and Implications  
**Subject:** CRS – Artificial Intelligence  
**Student:** Aditya Jitendra Kumar Sahani  
**Grade:** 11  
**School:** Aspee Nutan Academy  
**Student ID:** 1000414  

---

## 1. Live Chatbot Access

Interact with the deployed Smart Campus Assistant here:

**[https://console.dialogflow.com/api-client/demo/embedded/a28d1336-20b5-4e73-a544-6d009bce8762](https://console.dialogflow.com/api-client/demo/embedded/a28d1336-20b5-4e73-a544-6d009bce8762)**

---

## 2. Project Overview

This Smart Campus Assistant is an AI chatbot built in **Google Dialogflow ES** for the CRS Summative Assessment. It is designed to make all campus information instantly accessible, serving as a 24/7 self-service helpdesk for students, staff, and visitors.

The chatbot provides fast, automated responses to the most common campus queries, reducing dependency on manual inquiry. It is designed to meet the project's "Distinguished" criteria by implementing **19 intents** and **10 custom entities**.

It answers complex queries related to:
- **Academic Timetables** for specific programs and years
- **Admissions** processes and deadlines
- **Fee Payments** and accepted modes
- **Department & Faculty** contact information
- **Campus Navigation** to specific areas and buildings
- **Event Schedules** and locations
- **Hostel & Library** rules and timings
- **Emergency** contacts

---

## 3. Target Users

| User Group | Purpose |
| :--- | :--- |
| **New Students** | Orientation & campus familiarity |
| **Existing Students** | Quick access to timetables, fees, and contacts |
| **Parents & Visitors** | Guidance and navigation support |
| **Staff & Administration**| A tool for consistent and reliable communication |

---

## 4. Key AI Features & Design

- **Platform:** Developed using **Google Dialogflow Essentials (ES)**.
- **Intent Recognition:** Utilizes **19 distinct intents** to understand a wide variety of user requests.
- **Entity Extraction:** Employs **10 custom entities** (e.g., `@course_program`, `@campus_area`, `@doc_type`) to extract specific values from user speech.
- **Slot-Filling (Required Parameters):** Ensures all required information is collected. For example, the `Timetable Query` intent will prompt the user for their `@course_program` and `@year_level` if not provided.
- **Contextual Conversation:** Uses **Input/Output Contexts** to create multi-turn conversations. For example, after finding a department, the bot asks for a follow-up ("Would you like the email or phone?"), demonstrating conversational memory.
- **Rich Responses:** Uses **Suggestion Chips** (`[Library]`, `[Cafeteria]`) and **Quick Replies** to guide the user and make the conversation faster and more intuitive.
- **Static Database:** Provides information (like timetables) from a static PDF, a practical solution for a no-code project.

---

## 5. List of Intents (19 Total)

| Intent Name | Purpose |
| :--- | :--- |
| 1. **Welcome** | Greets the user and starts the conversation. |
| 2. **Fallback** | Handles queries the bot doesn't understand. |
| 3. **Goodbye** | Ends the session politely and asks for feedback. |
| 4. **Timetable Query** | (Slot-Filling) Provides the PDF link for a specific `@course_program` and `@year_level`. |
| 5. **Fees & Payment** | Details fee structure and accepted `@payment_mode` values. |
| 6. **Admissions Process** | Explains how to apply, deadlines, and requirements. |
| 7. **Course Information** | Provides syllabus links for a given `@course_program`. |
| 8. **Department Contacts** | (Uses Context) Finds a `@department` and asks for follow-up (email/phone). |
| 9. **Events & Notices** | Lists upcoming events, filtering by `@event_type` or `@sys.date`. |
| 10. **Library Services** | Provides details on a specific `@library_item` (e.g., fines, renewal, hours). |
| 11. **Campus Map / Navigation**| (Slot-Filling) Gives directions to a specific `@campus_area`. |
| 12. **Transport & Bus Routes**| Provides the link to the bus schedule. |
| 13. **Hostel / Accommodation**| Answers questions about a specific `@hostel_item` (e.g., mess timings, curfew). |
| 14. **Cafeteria / Food Services**| Gives the hours and menu details for the campus cafes. |
| 15. **Clubs & Student Bodies**| Explains how to join student clubs. |
| 16. **Documents & Certificates**| (Slot-Filling) Explains how to get a specific `@doc_type` (e.g., bonafide, ID card). |
| 17. **Emergency & Helpdesk**| Provides critical contact numbers for security and medical help. |
| 18. **Placements & Internships**| Gives information on the Training & Placement (T&P) cell. |
| 19. **IT Support (Wi-Fi/Email)**| Helps with Wi-Fi passwords and IT helpdesk contact. |

---

## 6. List of Custom Entities (10 Total)

| Entity Name | Used For Capturing (Examples) |
| :--- | :--- |
| **`@course_program`** | `B.Tech`, `BBA`, `MBA` (with synonyms like `Bachelor of Technology`) |
| **`@department`** | `Computer Science`, `Admissions`, `Accounts` (with synonyms like `CSE`, `finance office`) |
| **`@event_type`** | `workshop`, `seminar`, `fest` (with synonyms like `techfest`) |
| **`@time_slot`** | `morning`, `afternoon`, `evening` (with synonyms like `AM`, `post-lunch`) |
| **`@campus_area`** | `library`, `admin block`, `cafeteria` (with synonyms like `canteen`, `food court`) |
| **`@payment_mode`** | `UPI`, `card`, `net banking` (with synonyms like `Google Pay`, `debit card`) |
| **`@doc_type`** | `ID card`, `bonafide`, `transcripts` (with synonyms like `i-card`, `hall ticket`) |
| **`@hostel_item`** | `mess timing`, `curfew time`, `visitor pass` (with synonyms like `in-time`, `guest pass`) |
| **`@library_item`** | `due date`, `fine`, `renewal`, `book availability` (with synonyms like `late fee`, `find a book`) |
| **`@year_level`** | `1st year`, `2nd year`, `final year` (with synonyms like `first`, `second`, `3rd`) |

---

## 7. End-to-End Test Scenarios

The bot was validated against 5 end-to-end user journeys as required by the project rubric:

1.  **New Student Scenario:** `Hi` -> `How to apply for BBA?` -> `What is the fee?` -> `Where is the admin block?` -> `Thanks, bye!`
2.  **Existing Student (Timetable Test):** `Hello` -> `I need the schedule for BCA 2nd year` -> (Bot provides PDF link) -> `Also, where is the lab complex?` -> `Great, thanks.`
3.  **Library User Scenario:** `What are the library hours?` -> `How do I pay a library fine?` -> `How to renew a book?`
4.  **Context & Follow-up Scenario:** `Contact Admissions` -> (Bot asks for clarification) `Would you like their email or phone number?` -> `Email` -> (Bot provides email) -> `What about their phone?` -> (Bot provides phone).
5.  **Hostel Student Scenario:** `What's the curfew time?` -> `What are the mess timings?` -> `How do I get a visitor pass?`

---

## 8. Deployment Instructions

To deploy or reuse this chatbot agent:

1.  Open the **Dialogflow ES console**.
2.  **Export:** Go to the agent's **Settings (⚙️)** > **Export and Import** > **Export as ZIP**.
3.  **Import:** Create a new agent, go to its settings, and **Import from ZIP**.
4.  **Verify:** Check that all 19 intents and 10 entities have been imported correctly.
5.  **Customize:** Update the responses in each intent to include your school's specific URLs, phone numbers, and office locations.
6.  **Deploy:** Go to **Integrations** → Enable **Web Demo**.
7.  **Share:** Copy the generated web link and share it on the school website, in student emails, or on QR code posters around campus.

---

## 9. Future Improvements

-   **Voice Input:** Integrate Speech-to-Text for hands-free interaction.
-   **Dynamic Data:** Connect to a live database (via Fulfillment) to get real-time event updates and class schedules.
-   **Multi-language Support:** Add support for Hindi and other regional languages.
-   **Google Maps Integration:** Provide an interactive map with a pin for the requested location.

---

## 10. Collaboration

| Name | Student ID | Responsibility |
| :--- | :--- | :--- |
| **Aditya Jitendra Kumar Sahani** | 1000414 | Lead Development & Dialogflow Build |
| **Zene Sophie Anand** | 1000442 | Intent and Entity Structuring |
| **Naman Om Shreshta** | 1000432 | Testing, Debugging & Deployment Support |

---

### License
This project is created for educational and academic submission purposes under the WACP AI coursework.
