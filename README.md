#Use Case Documentation:

---

#USER USE CASES:

1. Register Account: The user creates an account with name, email, and password.
2. Login: The user logs into the system.
3. Browse Doctors: The user can browse a list of doctors based on specialization.
4. Send Consultation Request: The user sends a consultation request to a doctor.
5. View Request Status: The user can view the status of sent requests (pending/accepted/rejected).
6. Start Chat After Acceptance: The user can start chatting only if the doctor accepts the request.
7. Send Messages: The user can send messages (text, image, audio, PDF) to the doctor.
8. View Chat History: The user can view past chats.
9. Receive Notifications: The user receives system notifications (request updates, chat closed...).

---

#DOCTOR USE CASES:

1. Register Doctor Profile: The doctor registers with name, email, phone, and password.
2. Create Clinic Profile: The doctor sets up clinic information (name, location, description, optional photo).
3. Choose Specializations: The doctor selects the specializations they belong to.
4. Login: The doctor logs into the system.
5. View Incoming Requests: The doctor views received consultation requests.
6. Accept/Reject Request: The doctor accepts or rejects the request.
7. Start Chat After Acceptance: The doctor can chat only after accepting the request.
8. Send Messages: The doctor sends messages (text, image, voice, files).
9. Close Chat: The doctor can close the chat at any time.
10. Receive Notifications: The doctor receives alerts when new requests are received.

---

#ADMIN USE CASES:

1. Login: Admin logs into the system.
2. View Doctors: Admin sees all registered doctors.
3. Accept/Reject Doctors: Admin approves or rejects new doctor accounts.
4. Manage Specializations: Admin adds, edits, or deletes specializations.
5. View All Users: Admin views all registered users.
6. View Statistics: Admin checks system statistics (number of users, doctors, chats...).
7. Receive Notifications: Admin gets notified when a new doctor registers or when a user sends a consultation request.

---

#SYSTEM NOTIFICATIONS TABLE:

| Trigger                         | Notification Target | Content                                        |
| ------------------------------- | ------------------- | ---------------------------------------------- |
| User sends consultation request | Admin + Doctor      | "A new consultation request from User X"       |
| Doctor accepts/rejects request  | User                | "Your request was accepted/rejected by Dr. X"  |
| Doctor closes chat              | User                | "The chat has been closed by Dr. X"            |
| Doctor registers                | Admin               | "A new doctor has registered and needs review" |

---
