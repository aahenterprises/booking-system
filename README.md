# Online Booking System

A cloud-based appointment booking web app built by **AAH Enterprises**. Customers pick a service, date and time, and the owner manages every booking from a private admin panel.

## Features

**For customers (no login needed)**
- Choose a service, pick a date and select a free time slot
- Booked and past slots are disabled automatically
- Double booking is prevented, so two people cannot take the same slot
- Instant confirmation message after booking

**For the admin (login required)**
- Secure login with Firebase Authentication
- See all bookings in real time
- Confirm, cancel or delete bookings
- Cancelling or deleting a booking frees the slot again
- Search by name, phone, service or date, and filter by status
- Live cards: today's bookings, pending, confirmed and total

**General**
- Closed days and working hours are easy to change
- Loading logo animation and responsive green and gold design
- Works on phones, tablets and desktops

## Built with

- HTML5
- CSS3 (gradients, grid, animations)
- JavaScript (ES modules)
- Firebase Authentication
- Firebase Firestore (cloud database)

## How it works

Each time slot is saved as its own document with a fixed ID (for example `2026-10-20_1000`). Firestore does not allow a document with the same ID to be created twice, so a slot can only be booked once. Customer details are stored separately in `bookings`, and Firestore security rules allow only the admin to read them.

## How to run

1. Download or clone this repository.
2. Open `index.html` in a browser.
3. To use your own database, create a Firebase project, enable Email/Password sign-in and Firestore, replace the `firebaseConfig` values inside `index.html`, and publish the security rules.

## Customise

Open `index.html` and edit the `SETTINGS` section to change:
- the list of services
- working hours
- closed days

## Security note

The Firebase config in a web app is public by design. Data is protected by Firestore security rules: anyone can create a booking, but only the admin can read, confirm or delete bookings.

## Author

**Muhammad Awais Raza**, Founder & CEO, AAH Enterprises
Email: contact.aahenterprises@gmail.com
GitHub: [github.com/aahenterprises](https://github.com/aahenterprises)

&copy; 2026 AAH Enterprises<img width="1311" height="599" alt="Screenshot 2026-10-17 003751" src="https://github.com/user-attachments/assets/47f2d09f-c520-473c-8b4e-01dfcdff42da" />
<img width="1244" height="604" alt="Screenshot 2026-10-17 003841" src="https://github.com/user-attachments/assets/a4060804-a1d6-44f8-ad3e-e927dc72c4fa" />
<img width="1244" height="606" alt="Screenshot 2026-10-17 003909" src="https://github.com/user-attachments/assets/8c62af47-3e4f-40f0-b723-f6cd4fa56d2b" />
<img width="1251" height="522" alt="Screenshot 2026-10-17 003936" src="https://github.com/user-attachments/assets/762846a8-ebc3-4e13-a861-164f60df6cba" />
<img width="1116" height="524" alt="Screenshot 2026-10-17 004013" src="https://github.com/user-attachments/assets/725f4781-061a-499e-93c7-b9b3c21ad92b" />
<img width="1164" height="420" alt="Screenshot 2026-10-17 004045" src="https://github.com/user-attachments/assets/08c103b3-db07-47aa-bbea-cb9d841e3af6" />
<img width="1164" height="420" alt="Screenshot 2026-10-17 004045" src="https://github.com/user-attachments/assets/3b7951af-b993-49f2-85f7-024f8084383f" />
<img width="1118" height="458" alt="Screenshot 2026-10-17 004339" src="https://github.com/user-attachments/assets/c8293727-f7eb-4eec-98ef-d352fa2677d7" />
