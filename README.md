# SwiftShip Tracker

A Salesforce CRM application for parcel booking, shipment tracking, and delivery management. It centralizes Parcel, Delivery, Sender, and Receiver information and uses Salesforce Flow, Prompt Builder, and Agentforce AI to provide conversational parcel tracking.

**Program:** Salesforce Developer (Naan Mudhalvan)  
**College:** Arasu Engineering College, Kumbakonam  
**Project:** SwiftShip Tracker  
**Team Members: sanjay c, Abishek E, vishva B, sachin c, sanjay G

## Demo Video

**Watch the Demo Video:** `https://drive.google.com/file/d/1lfWLZ9J7rB3CGwUaXGTgEXQoOjUKuNXi/view?usp=sharing`

## Features

- Four custom objects: Parcel, Delivery, Sender, and Receiver
- Parcel booking and shipment tracking
- Delivery status management
- Sender and receiver information management
- Parcel Details Salesforce Flow
- Prompt Builder – Retrieve Parcel Details
- Agentforce AI – SwiftShip Tracker
- Conversational parcel tracking
- Role-based access control
- Permission Sets and Field-Level Security
- Reports and Dashboards
- Experience Cloud customer access
- Apex and Batch Apex components

## Salesforce Components

| Component | Implementation |
|---|---|
| Custom Objects | Parcel, Delivery, Sender, Receiver |
| Automation | Salesforce Flow |
| AI | Agentforce |
| Prompt | Retrieve Parcel Details |
| Security | Profiles, Roles, Permission Sets, Sharing Rules, FLS |
| UI | Lightning App / Experience Cloud |
| Analytics | Reports & Dashboards |
| Development | Apex / Batch Apex |

## Project Workflow

```text
Customer / Sender
        ↓
Parcel Booking
        ↓
Parcel Record
        ↓
Sender + Receiver
        ↓
Delivery Record
        ↓
Status Update
        ↓
Current Location + Estimated Delivery
        ↓
Automated Notification
        ↓
Customer Tracking / Agentforce AI
        ↓
Reports & Dashboards
```

## Agentforce Workflow

```text
User
  ↓
SwiftShip Tracker Agentforce Agent
  ↓
Parcel Details Flow
  ↓
Get Parcel Record
  ↓
Retrieve Parcel Details Prompt
  ↓
Prompt Response
  ↓
Agentforce Response
```

## Custom Objects

### Parcel
Stores Parcel ID, Status, Weight, Estimated Delivery Date, Sender and Receiver relationships.

### Delivery
Stores Current Location, Estimated Delivery Date, Sender and Parcel relationships.

### Sender
Stores Sender Address, Sender Contact and Sender Email.

### Receiver
Stores Receiver Address, Receiver Contact, Receiver Email, Sender and Parcel relationships.

## Prompt Builder

**Template:** Retrieve Parcel Details

The prompt uses parcel information including:

- Parcel Name
- Parcel ID
- Status
- Weight
- Estimated Delivery Date

## Salesforce Flow

**Flow:** Parcel Details

The documented flow follows:

```text
Start
  ↓
Get Parcel Records
  ↓
Parcel Updates / Prompt Action
  ↓
Assignment Outputs
  ↓
End
```

Input variable: `ids`  
Output variable: `Output`

## Security

The project uses Salesforce:

- Profiles
- Roles
- Permission Sets
- Sharing Rules
- Field-Level Security

The documented role model includes Administrator, Delivery Manager, Agent, Customer and Support Staff.

## Repository Contents

```text
SwiftShip-Tracker/
│
├── Code/
│   ├── Apex Classes/
│   ├── Apex Triggers/
│   ├── Batch Apex/
│   ├── Flows/
│   ├── Custom Objects/
│   ├── Permission Sets/
│   ├── Agentforce/
│   ├── Prompt Builder/
│   └── Reports and Dashboards/
│
├── README.md
├── SwiftShip-Tracker-Project-Report.pdf
└── SwiftShip-Tracker-Project-Report.docx
```

## Documentation

The repository contains the project report and implementation documentation. Actual Salesforce metadata should be exported from the Salesforce org and placed inside the corresponding `Code` folders before using this repository as a deployable source repository.

## Future Scope

- Extend Agentforce for more parcel-management queries
- Improve real-time delivery tracking
- Expand Experience Cloud self-service
- Add advanced delivery-performance analytics
- Integrate external courier and logistics systems
- Improve AI prompts and conversational experiences
- Introduce enterprise sandbox and CI/CD deployment

## Team

**sanjay c** – Project Member  
**Sachin c** – Project Member
**vishva B** – Project Member
**sanjay G** – Project Member
**abishek E** – Project Member
