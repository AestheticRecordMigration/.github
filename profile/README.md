# AESTHETICRECORD.COM

# Setup for developers
- Install the requirements from req.txt file
- Repositories are build on top of python3, django, scrapy at the core.

## Servers for development
- Server 1: ubuntu@35.83.137.252
- Server 2: ubuntu@34.213.205.112

To get access to the servers, your have to first generate SSH keys for your system and then someone at AR has to give access to those keys.

## Repository

### migration-api
- This repository contains all code related to the apis. 
- We have api's for inventory, services, variation, giftcards, promotions or packages, patient demographics, documents, notes, appointments, procedures.
- In case if need to explore aestheticrecord.com api's to update this repo, then we can refer to postman collection of AR api's 
https://aestheticrecord.postman.co/

### migration-scripts
- This repository contains code related to the scripts.
- We have scripts for uploading data to AR and scraping data from various platforms.
- We can also refer to this sheet to get an idea about what fields we have to scrape: https://docs.google.com/spreadsheets/d/1GGxgO3N0-01nYM2KvLEhJWYypLJ_dCgvrcV77plNdT0/edit#gid=956186815


## Types of Tasks

### Configure and Deliver (C/D)
Under this head of tasks, we have tasks to upload data to AR generally from excel sheets or csv.
We have scripts for
- Inventory
- Services
- Inventory Variation
- Promotions/Packages
- Gift Cards
- Patient Demographics
- Appointments
- Documents
- Notes
- Wallet Items
- Exporting Procedures

### Data Migration (D/M)
Under this head of tasks, we have to follow a 3 step process. Scraping data from a system -> Storing data in server or local -> Migrating the stored data to AR.

### Data we can get

#### Myaestheticspro
- Patient Demographics
- Documents: Invoices, Photos
- Notes
- Some of the documents
- Past & Future Appointments

#### Booksy
- Patient Demographics
- Past & Future Appointments
- Notes: Client Note

#### Practicefusion
- Patient Demographics
- Past & Future Appointments
- Documents: Signed, Pending
- Notes: Client Pinned Note, Client Profile Note, encounter attachments, Allergies, Diagnoses, Medications, patientGoals, Messages, Advanced Directives, Patient Risk Score, PersonalMedicalHistory, socialhealth, behaviour health

#### Meevo
- Patient Demographics
- Past & Future Appointments
- Notes
- Documents: Images

#### Drchrono
- Patient Demographics
- Past & Future Appointments
- Documents: Locked Clinical NOte, documents
- Notes: Problem List, Medication List, Allergy List, Drug Interactions

#### Rxphoto
- Patient Demographics
- Notes: Comments
- Documents: Images

#### Janeapp
- Patient Demographics
- Past & Future Appointments
- Notes: Medical Alert, Chart
- Documents: Patient files, Notes, Invoices/Billing

#### Daysmartspa/Mindbodyonline/crystalcleardm
- Patient Demographics
- Past & Future Appointments
- Notes: ClientNoteList
- Documents: Photos

#### Cpsurgeons
- Patient Demographics
- Past & Future Appointments
- Documents: Labs, Radiology, Miscellaneous,MedicalClearance, PatientIntake, PreSymplastEMR, PatientConsentForms
