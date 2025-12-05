# Database Design for Online Event Registration System

## 1. Tables Required

### **1. Events Table**
| Column Name     | Type        | Description                     |
|-----------------|-------------|---------------------------------|
| event_id        | INT / AUTO  | Unique ID for each event       |
| event_name      | VARCHAR     | Name of the event              |
| description     | TEXT        | Event description              |
| date            | DATE        | Event date                     |
| time            | TIME        | Event time                     |
| venue           | VARCHAR     | Location of event              |

### **2. Users / Participants Table**
| Column Name     | Type        | Description                     |
|-----------------|-------------|---------------------------------|
| user_id         | INT / AUTO  | Unique ID for each user        |
| name            | VARCHAR     | Participant name               |
| email           | VARCHAR     | Email ID                       |
| phone           | VARCHAR     | Mobile number                  |

### **3. Registrations Table**
| Column Name     | Type        | Description                     |
|-----------------|-------------|---------------------------------|
| registration_id | INT / AUTO  | Unique ID for each registration|
| user_id         | INT (FK)    | Participant                    |
| event_id        | INT (FK)    | Event registered               |
| timestamp       | DATETIME    | Registration time              |

## 2. ER Diagram (Text Form)
