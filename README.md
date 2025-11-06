# Smart Campus Assistant  
AI-Based Conversational Guide for Campus Navigation & Support

**Course:** Artificial Intelligence – Real-World Applications and Implications  
**Subject:** CRS – Artificial Intelligence  
**Student:** Aditya Jitendra Kumar Sahani  
**Grade:** 11  
**School:** Aspee Nutan Academy  
**Student ID:** 1000414  

---

## 1. Live Chatbot Access

Interact with the deployed Smart Campus Assistant here:

**[Smart Campus Assistant](https://console.dialogflow.com/api-client/demo/embedded/a28d1336-20b5-4e73-a544-6d009bce8762)**

---

## 2. Project Overview

The Smart Campus Assistant is a Dialogflow-based AI chatbot designed to make campus information easier to access.  
It provides fast, automated responses to commonly asked questions related to campus navigation, staff offices, event schedules, services, and emergency information.  
The chatbot reduces dependency on manual inquiry and serves as a **24/7 self-service helpdesk**.

It answers queries like:
- Locations of academic buildings and labs  
- Faculty office and department details  
- Facility and office operating hours  
- Event schedules and venue information  
- Transportation options within and near campus  
- Emergency support and contact numbers  

---

## 3. Target Users

| User Group | Purpose |
|---|---|
| New Students | Orientation & campus familiarity |
| Existing Students | Quick access to repeated information |
| Parents & Visitors | Guidance and navigation support |
| Staff & Administration | Consistent and reliable communication |

---

## 4. Integration Details

- Developed using **Google Dialogflow Essentials**.
- **Intents** identify what the user is asking.
- **Entities** extract specific information (such as building names or professor names).
- **Slot Filling** ensures the chatbot collects missing details before answering (e.g., asks for professor name if not provided).
- **Training Phrases** improve understanding of natural variations in queries.
- **Rich Responses** (suggestion chips, quick replies, images) improve clarity and usability.
- Hosted using Dialogflow’s **Web Demo Integration**. No external APIs required.

---

## 5. List of Intents (15)

| Intent Name | Purpose |
|---|---|
| Default Welcome | Start conversation and greet user |
| Default Fallback | Handle unclear queries |
| find_academic_building | Locate academic departments or blocks |
| find_event | Provide event schedule/location |
| find_hours | Provide office or facility timings |
| find_lab | Directions to science/CS labs |
| find_location | Locate general campus places |
| find_professor_office | Provide professor office location |
| find_service_building | Locate services like library/admin/hostel |
| get_contact | Provide phone/email of a department |
| get_emergency_contact | Provide emergency support contact |
| get_nearby_recreation | Suggest recreational or refreshment places |
| get_policy | Explain campus policies and rules |
| get_transportation | Provide bus/transport details |
| Goodbye | Ends the session politely |

---

## 6. Custom Entities (10)

| Entity Name | Used For Capturing |
|---|---|
| `@academic_building` | Building/department names |
| `@contact_type` | Phone / Email / Address |
| `@event_name` | Event identifiers |
| `@facility` | Facilities like cafeteria/gym |
| `@lab_name` | Lab names |
| `@location` | General campus areas |
| `@policy_type` | Policy categories |
| `@professor_name` | Instructor/faculty names |
| `@recreation_type` | Recreation place types |
| `@service_building` | Library / Admin / Hostel / Admissions |

---

## 7. Deployment Instructions

To deploy or reuse the chatbot:

1. Open Dialogflow: `https://dialogflow.cloud.google.com/`
2. Import or create the Smart Campus Assistant agent.
3. Add all intents and entities listed above.
4. Verify training phrases and responses.
5. Go to **Integrations** → Enable **Web Demo**.
6. Copy the generated web link or embed code.
7. Share the link on:
   - School website
   - Student onboarding handbook
   - QR code posters around campus

Deployment is complete when the chatbot responds live in the browser.

---

## 8. Deployment Status

- Fully deployed  
- Accessible across devices  
- Works without login  
- No additional installation required  

---

## 9. Future Improvements

- Add voice input (Speech → Text)
- Connect interactive campus map for live navigation
- Add multi-language support

---

## 10. Collaboration

| Name | Student ID | Responsibility |
|---|---|---|
| Aditya Jitendra Kumar Sahani | 1000414 | Lead Development & Dialogflow Build |
| Zene Sophie Anand | 1000442 | Intent and Entity Structuring |
| Naman Om Shreshta | 1000432 | Testing, Debugging & Deployment Support |

---

### License
This project is created for educational and academic submission purposes under the WACP AI coursework.

