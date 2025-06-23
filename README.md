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
توثيق حالات الاستخدام (Use Case Documentation)

---

📌 حالات استخدام المستخدم (User):

1. تسجيل حساب: يقوم المستخدم بإنشاء حساب جديد باستخدام الاسم، البريد الإلكتروني، وكلمة المرور.
2. تسجيل الدخول: يسجل المستخدم الدخول إلى النظام.
3. تصفح الأطباء: يمكن للمستخدم تصفح قائمة الأطباء حسب التخصص.
4. إرسال طلب استشارة: يرسل المستخدم طلبًا إلى طبيب معين.
5. عرض حالة الطلب: يعرض المستخدم حالة طلبه (معلق / مقبول / مرفوض).
6. بدء المحادثة بعد القبول: لا يمكن للمستخدم بدء المحادثة إلا بعد قبول الطبيب للطلب.
7. إرسال رسائل: يرسل المستخدم رسائل (نصوص، صور، صوت، ملفات PDF).
8. عرض سجل المحادثات: يمكن للمستخدم مراجعة المحادثات السابقة.
9. استقبال الإشعارات: يتلقى المستخدم تنبيهات من النظام (تغييرات حالة الطلب أو إغلاق المحادثة).

---

📌 حالات استخدام الطبيب (Doctor):

1. تسجيل حساب طبيب: يقوم الطبيب بالتسجيل باستخدام الاسم، البريد الإلكتروني، رقم الهاتف، وكلمة المرور.
2. إنشاء ملف العيادة: يملأ الطبيب بيانات العيادة (الاسم، الموقع، الوصف، صورة اختيارية).
3. اختيار التخصصات: يحدد الطبيب التخصصات التي يعمل بها.
4. تسجيل الدخول: يسجل الطبيب الدخول إلى النظام.
5. عرض الطلبات الواردة: يشاهد الطبيب طلبات الاستشارة المرسلة إليه.
6. قبول / رفض الطلب: يتخذ الطبيب قرار قبول أو رفض الطلب.
7. بدء المحادثة بعد القبول: يبدأ الطبيب المحادثة فقط بعد قبول الطلب.
8. إرسال رسائل: يرسل الطبيب رسائل (نصوص، صور، ملفات صوتية أو PDF).
9. إغلاق المحادثة: يمكن للطبيب إنهاء المحادثة في أي وقت.
10. استقبال الإشعارات: يتلقى الطبيب إشعارات عند وصول طلب جديد.

---

📌 حالات استخدام المدير (Admin):

1. تسجيل الدخول: يسجل المدير الدخول إلى لوحة التحكم.
2. عرض الأطباء: يمكن للمدير عرض جميع حسابات الأطباء المسجلين.
3. قبول / رفض الأطباء: يوافق أو يرفض حسابات الأطباء الجديدة.
4. إدارة التخصصات: يضيف أو يعدل أو يحذف تخصصات من النظام.
5. عرض المستخدمين: يمكنه عرض جميع المستخدمين المسجلين.
6. عرض الإحصائيات: يطّلع المدير على بيانات تحليلية (عدد المستخدمين، عدد الأطباء، عدد المحادثات...).
7. استقبال الإشعارات: يتلقى إشعارات عندما يسجل طبيب جديد أو يرسل مستخدم طلب استشارة.

---

📌 جدول الإشعارات (Notifications Table):

| الحدث                     | من يستقبل الإشعار | محتوى الإشعار                                 |
| ------------------------- | ----------------- | --------------------------------------------- |
| المستخدم يرسل طلب استشارة | المدير + الطبيب   | "تم استقبال طلب استشارة جديد من المستخدم X"   |
| الطبيب يقبل أو يرفض الطلب | المستخدم          | "تم قبول / رفض طلبك من الطبيب X"              |
| الطبيب يغلق المحادثة      | المستخدم          | "قام الطبيب X بإغلاق المحادثة"                |
| تسجيل طبيب جديد           | المدير            | "طبيب جديد سجل في النظام ويحتاج إلى الموافقة" |

---
✅ الخطوات التالية بعد تجهيز قاعدة البيانات:
🔧 1. إنشاء Auth System للمستخدم، الطبيب، المدير
كل واحد له تسجيل دخول منفصل:

User: Register/Login

Doctor: Register/Login + Approval by admin

Admin: Login only (no register)

✅ الأفضل: استعمل Laravel Fortify أو Sanctum لتأمين الـ API.

📦 2. بناء API كاملة (REST أو JSON API) لكل Use Case:
رتبتهم لك على شكل مهام جاهزة:

👤 User Endpoints (API)
الوظيفة	الميثود	Endpoint
تسجيل حساب	POST	/api/user/register
تسجيل دخول	POST	/api/user/login
استعراض الأطباء	GET	/api/doctors?specialization=...
إرسال طلب استشارة	POST	/api/consultations
عرض الطلبات	GET	/api/user/consultations
بدء المحادثة (بعد القبول)	GET	/api/chat/{consultation_id}
إرسال رسالة	POST	/api/messages
رفع صورة / ملف	POST	/api/messages/upload
استعراض المحادثات	GET	/api/user/chats
الإشعارات	GET	/api/user/notifications

🧑‍⚕️ Doctor Endpoints (API)
الوظيفة	الميثود	Endpoint
تسجيل حساب	POST	/api/doctor/register
تسجيل دخول	POST	/api/doctor/login
إنشاء العيادة	POST	/api/clinic
اختيار التخصصات	POST	/api/doctor/specializations
عرض الطلبات	GET	/api/doctor/consultations
قبول / رفض الطلب	POST	/api/consultations/{id}/respond
بدء المحادثة	GET	/api/chat/{consultation_id}
إرسال رسالة	POST	/api/messages
إغلاق المحادثة	POST	/api/chat/{id}/close
الإشعارات	GET	/api/doctor/notifications

🛠️ Admin Endpoints
الوظيفة	الميثود	Endpoint
تسجيل دخول	POST	/api/admin/login
عرض الأطباء	GET	/api/admin/doctors
قبول / رفض طبيب	POST	/api/admin/doctors/{id}/status
عرض المستخدمين	GET	/api/admin/users
إدارة التخصصات	GET/POST/PUT/DELETE	/api/admin/specializations
عرض الإحصائيات	GET	/api/admin/stats
الإشعارات	GET	/api/admin/notifications

📌 3. إرسال الإشعارات (notifications)
❗ مهم: كل Endpoint مرتبط بـ Notification لازم يدعم إرسال إشعار فورًا:

عند تسجيل الطبيب → إشعار للإدمن

عند إرسال طلب → إشعار للطبيب + الإدمن

عند قبول / رفض الطلب → إشعار للمستخدم

عند إغلاق المحادثة → إشعار للمستخدم

✅ حطها داخل NotificationService class أو استخدم Laravel Events & Listeners.

🛡️ 4. تأمين API عبر Sanctum أو Passport
كل من:

User

Doctor

Admin
يحتاج حماية خاصة بتوكيناته عشان تعرف كل واحد وصلاحياته.

✅ Laravel Sanctum هو الأبسط.

✅ 5. التوثيق الجاهز لفريق Flutter
سوِّ لهم:

Postman Collection (كل Endpoints + Sample Response)

أو Swagger/OpenAPI إن قدرت

🧠 نصيحة عملية
ابدأ حسب الأولوية:

User auth

Doctor auth

Consultation flow (Send / Accept / Reject)

Messaging

Notifications

Admin Panel APIs
