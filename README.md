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

[Smart Campus Assistant](https://console.dialogflow.com/api-client/demo/embedded/a28d1336-20b5-4e73-a544-6d009bce8762)

---

## 2. Project Summary

The Smart Campus Assistant is a chatbot developed using **Google Dialogflow**. It provides quick, reliable campus-related information to students, staff, parents, and visitors. The chatbot replaces repeated manual queries with instant automated responses.

It handles:
- Building and department locations  
- Faculty office details  
- Facility opening hours  
- Event schedules  
- Emergency contacts  
- Campus transportation and services  

This system functions as a **self-service campus helpdesk** available at all times.

---

## 3. Target Users

| User Group | Primary Need |
|---|---|
| New Students | Orientation & directions |
| Existing Students | Quick recurring information |
| Parents & Visitors | Navigation and campus procedures |
| Staff | Streamlined communication |

---

## 4. System Details

**Platform Used:** Dialogflow Essentials  
**Core Features:**
- Natural Language Understanding (NLU)
- Intent and Entity-based query handling
- Slot filling for multi-step responses
- Rich Responses (chips, maps, images)

---

## 5. Intents (15)

| Intent Name | Purpose |
|---|---|
| Default Welcome | Greets the user |
| Default Fallback | Handles unknown queries |
| find_academic_building | Locate academic buildings |
| find_event | Event time/location info |
| find_hours | Facility operating hours |
| find_lab | Directions to campus labs |
| find_location | General campus directions |
| find_professor_office | Locate professor offices |
| find_service_building | Locate service buildings |
| get_contact | Provide department contact info |
| get_emergency_contact | Provide emergency numbers |
| get_nearby_recreation | Suggest recreation spaces |
| get_policy | Explain campus policies |
| get_transportation | Transportation details |
| Goodbye | Close conversation |

---

## 6. Entities (10)

| Entity Name | Captures |
|---|---|
| `@academic_building` | Academic block names |
| `@contact_type` | Phone / Email / Address |
| `@event_name` | Event identifiers |
| `@facility` | Facilities like gym/cafeteria |
| `@lab_name` | Science/CS lab names |
| `@location` | General campus locations |
| `@policy_type` | Policy categories |
| `@professor_name` | Faculty names |
| `@recreation_type` | Cafe / park / etc. |
| `@service_building` | Service building names |

---

## 7. Deployment Status

- Chatbot fully functional  
- Hosted online via Dialogflow  
- Accessible through browser  
- Works on desktop and mobile  

---

## 8. Future Improvements

- Add voice input support  
- Integrate campus map navigation  
- Add multilingual support  

---

### License
This project is submitted as part of the school coursework for educational demonstration.

