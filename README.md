# Smart India Hackathon Workshop
# Date: 18/09/26
## Register Number: 212225230083
## Name: GOPIKA DHARSHINI.N

## Problem Title
SIH 1710: Enhancing Navigation for Railway Station Facilities and Locations

## Problem Description
Background: Railway stations are complex environments with numerous facilities and locations such as ticket counters, platforms, restrooms, food courts, and waiting areas. Passengers often face difficulties in navigating these spaces, especially in large or unfamiliar stations. Efficient and user-friendly navigation systems are crucial for improving passenger experience, reducing congestion, and ensuring timely travel connections. Description: The problem involves developing a comprehensive navigation solution for railway stations that assists passengers in locating various facilities and destinations within the station premises. This includes creating detailed maps, providing real-time directions, and integrating features such as accessibility options for individuals with disabilities. The solution should be intuitive, easy to use, and accessible via multiple platforms, including mobile devices and digital kiosks. Key challenges include updating navigation information in real-time, ensuring accuracy, and accommodating the diverse needs of all passengers. Expected Solution: The expected solution is a multi-platform navigation system that provides detailed, real-time directions to all facilities and locations within a railway station. This system should include: A mobile application with 3D interactive maps and step-by-step navigation. Digital kiosks located throughout the station with touch-screen interfaces. Voice-guided navigation for visually impaired passengers. Regular updates to reflect changes in station layout and facility locations. Integration with existing railway apps and services for seamless user experience. The solution should enhance the overall passenger experience by reducing confusion, saving time, and improving accessibility within the station.

## Problem Creater's Organization
Ministry of Railway

## Idea
RailNav AI – Smart Indoor Railway Station Navigation System

RailNav AI is an AI-powered indoor navigation system designed to help passengers quickly locate platforms, ticket counters, restrooms, food courts, waiting halls, lifts, escalators, exits and other railway facilities.

Unlike conventional map applications, RailNav AI focuses specifically on the complex indoor environment of railway stations. It provides step-by-step navigation, accessibility-aware routes, voice guidance and AI-based route selection.

The system can understand the passenger's requirement and provide the most suitable route based on:

Current location
Destination
Walking distance
Crowd level
Accessibility requirements
Platform changes
Temporary blockages
Available lifts/escalators
Passenger's preferred route

## Proposed Solution / Architecture Diagram
                 ┌─────────────────────────┐
                 │       PASSENGER         │
                 │ Mobile App / Kiosk      │
                 └────────────┬────────────┘
                              │
                              ▼
                 ┌─────────────────────────┐
                 │    USER INPUT LAYER     │
                 │                         │
                 │ • Current Location      │
                 │ • Destination           │
                 │ • Accessibility Needs   │
                 │ • Route Preference      │
                 └────────────┬────────────┘
                              │
                              ▼
                 ┌─────────────────────────┐
                 │       AI ENGINE         │
                 │                         │
                 │ • Route Selection       │
                 │ • Crowd Analysis        │
                 │ • Accessibility Check   │
                 │ • Facility Detection    │
                 └────────────┬────────────┘
                              │
                    ┌─────────┴─────────┐
                    ▼                   ▼
          ┌─────────────────┐   ┌─────────────────┐
          │ Indoor Map DB   │   │ Real-Time Data  │
          │                 │   │                 │
          │ • Platforms     │   │ • Crowd Level   │
          │ • Facilities    │   │ • Closures      │
          │ • Lifts         │   │ • Platform Info │
          │ • Stairs        │   │ • Updates       │
          └────────┬────────┘   └────────┬────────┘
                   │                     │
                   └──────────┬──────────┘
                              ▼
                 ┌─────────────────────────┐
                 │   NAVIGATION ENGINE     │
                 │                         │
                 │ Shortest / Accessible   │
                 │ / Easy / Low-Crowd      │
                 └────────────┬────────────┘
                              │
                              ▼
              ┌──────────────────────────────┐
              │       OUTPUT LAYER           │
              │                              │
              │ 🗺 Interactive Map            │
              │ 🧭 Step-by-Step Directions   │
              │ 🔊 Voice Guidance            │
              │ 📱 Mobile Navigation         │
              │ 🖥 Digital Kiosk             │
              └──────────────────────────────┘

## Use Cases
1. Passenger Navigation

A passenger enters:

"Platform 7"

The system identifies the current location and displays the route to Platform 7.

2. Facility Search

The passenger can search for:

Restroom
Ticket counter
Food court
Waiting hall
Drinking water
Medical facility
Lift
Escalator
Exit
Cloakroom
3. Accessibility Navigation

A passenger using a wheelchair can select Accessible Mode.

The system avoids:

Stairs
Narrow passages
Inaccessible entrances

and prioritizes:

Lifts
Ramps
Accessible paths.
4. Voice Navigation

Visually impaired passengers receive voice instructions for navigation.

For example:

"Move straight for 20 metres and take the lift on your left."

5. Platform Navigation

If the passenger needs to move from Platform 2 to Platform 8, the system provides the appropriate internal route instead of simply showing the station location.

6. AI-Based Route Selection

If multiple routes are available, the AI engine can compare them based on:

Distance
Estimated walking time
Accessibility
Crowd level
Temporary restrictions

and generate an appropriate route.

7. Digital Kiosk

Passengers who do not have the mobile application can use touchscreen kiosks installed inside the station.

They can select:

Current Location → Destination → Route Mode → Start Navigation

8. Emergency Navigation

The system can provide routes towards:

Emergency exits
Medical facilities
Railway help desks
Security offices

during emergency situations.

## Technology Stack

| Component                   | Technology                          |
| --------------------------- | ----------------------------------- |
| **Mobile Application**      | React Native / Flutter              |
| **Web/Kiosk Interface**     | React.js                            |
| **Frontend**                | HTML, CSS, JavaScript               |
| **Backend**                 | Python / FastAPI                    |
| **AI/ML**                   | Python, Scikit-learn                |
| **Navigation Algorithm**    | Dijkstra / A*                       |
| **Database**                | Firebase / PostgreSQL               |
| **Indoor Maps**             | OpenStreetMap / Custom Station Maps |
| **Location Detection**      | QR / Bluetooth Beacon / Wi-Fi       |
| **Voice Navigation**        | Text-to-Speech                      |
| **AI Processing**           | Python                              |
| **Real-Time Communication** | Firebase / WebSockets               |
| **Deployment**              | Firebase / Render / AWS             |


## Dependencies

Software Dependencies
Python 3.x
Node.js
React.js / React Native
FastAPI
Firebase
PostgreSQL
OpenStreetMap
Git & GitHub
VS Code
Web browser
Python Libraries
NumPy
Pandas
Scikit-learn
NetworkX
FastAPI
Uvicorn
Frontend Dependencies
React
React Router
Leaflet
Axios
Hardware Dependencies

For the prototype:

Laptop/PC
Android smartphone
QR codes
Optional Bluetooth Beacons
Optional touchscreen display for kiosk prototype
