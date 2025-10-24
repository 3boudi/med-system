###Use Case Documentation:

---

##USER USE CASES:

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

##DOCTOR USE CASES:

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

##ADMIN USE CASES:

1. Login: Admin logs into the system.
2. View Doctors: Admin sees all registered doctors.
3. Accept/Reject Doctors: Admin approves or rejects new doctor accounts.
4. Manage Specializations: Admin adds, edits, or deletes specializations.
5. View All Users: Admin views all registered users.
6. View Statistics: Admin checks system statistics (number of users, doctors, chats...).
7. Receive Notifications: Admin gets notified when a new doctor registers or when a user sends a consultation request.

---

##SYSTEM NOTIFICATIONS TABLE:

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

## 🚀 Features

- **Real-time Messaging** - Live chat between users and doctors
- **Multi-role Authentication** - Separate authentication for users, doctors, and admins
- **Doctor Approval Workflow** - Admin-controlled doctor registration approval
- **Medical Specializations** - 37 medical specialties with doctor categorization
- **Consultation Management** - Request, accept, and manage medical consultations
- **File Sharing** - Support for text, image, and file messages
- **Email Verification** - Secure user registration with email confirmation
- **Google OAuth** - Social authentication for users
- **Clinic Management** - Doctor clinic information and details
- **Notification System** - Polymorphic notifications for all user types

## 🗄️ Database Schema

### Tables and Their Attributes

#### Core Authentication & System Tables
- **users**
  - `id` (primary key), `name`, `email` (unique), `email_verified_at`, `password`, `remember_token`, `timestamps`

- **password_reset_tokens**
  - `email` (primary key), `token`, `created_at`

- **sessions**
  - `id` (primary key), `user_id`, `ip_address`, `user_agent`, `payload`, `last_activity`

- **personal_access_tokens**
  - `id`, `tokenable_id`, `tokenable_type`, `name`, `token` (unique), `abilities`, `last_used_at`, `expires_at`, `timestamps`

#### Queue & Cache Tables
- **cache** - `key` (primary key), `value`, `expiration`
- **cache_locks** - `key` (primary key), `owner`, `expiration`
- **jobs** - `id`, `queue`, `payload`, `attempts`, `reserved_at`, `available_at`, `created_at`
- **job_batches** - `id` (primary key), `name`, `total_jobs`, `pending_jobs`, `failed_jobs`, `failed_job_ids`, `options`, `cancelled_at`, `created_at`, `finished_at`
- **failed_jobs** - `id`, `uuid` (unique), `connection`, `queue`, `payload`, `exception`, `failed_at`

#### Healthcare Domain Tables
- **admins**
  - `id`, `name`, `email` (unique), `email_verified_at`, `password`, `remember_token`, `timestamps`

- **doctors**
  - `id`, `name`, `email` (unique), `password`, `phone`, `status` (enum: pending, accepted, rejected), `clinic_id` (foreign key), `remember_token`, `timestamps`

- **specializations**
  - `id`, `specialization` (unique), `timestamps`

- **clinics**
  - `id`, `name` (unique), `location`, `description`, `photo`, `timestamps`

- **consultation_requests**
  - `id`, `user_id` (foreign key), `doctor_id` (foreign key), `status` (enum: pending, accepted, rejected), `created_at`, `responded_at`

- **chats**
  - `id`, `consultation_request_id` (unique, foreign key), `is_closed`, `closed_at`, `timestamps`

- **messages**
  - `id`, `chat_id` (foreign key), `sender_type` (enum: user, doctor), `sender_id`, `type` (enum: text, image, file), `message`, `file_path` (JSON), `sent_at`, `timestamps`

- **notifications**
  - `id`, `notifiable_type`, `notifiable_id`, `type`, `data` (JSON), `read_at`, `created_at`

- **doctor_specialization** (pivot table)
  - `id`, `doctor_id` (foreign key), `specialization_id` (foreign key), `timestamps`

## 🔗 Database Relationships

### One-to-Many Relationships
- **clinics** → **doctors** - One clinic can have many doctors
- **users** → **consultation_requests** - One user can have many consultation requests
- **doctors** → **consultation_requests** - One doctor can have many consultation requests
- **chats** → **messages** - One chat can have many messages

### One-to-One Relationships
- **consultation_requests** → **chats** - One consultation request has exactly one chat

### Many-to-Many Relationships
- **doctors** ↔ **specializations** - Doctors can have multiple specializations via `doctor_specialization` pivot table

### Polymorphic Relationships
- **personal_access_tokens** - Can belong to users, doctors, or admins
- **messages** - Can be sent by users or doctors
- **notifications** - Can be sent to users, doctors, or admins

## 🗂️ Foreign Key Constraints

| Table | Foreign Key | References | On Delete |
|-------|-------------|------------|-----------|
| doctors | clinic_id | clinics.id | SET NULL |
| consultation_requests | user_id | users.id | CASCADE |
| consultation_requests | doctor_id | doctors.id | CASCADE |
| chats | consultation_request_id | consultation_requests.id | CASCADE |
| messages | chat_id | chats.id | CASCADE |
| doctor_specialization | doctor_id | doctors.id | CASCADE |
| doctor_specialization | specialization_id | specializations.id | CASCADE |

## 🏥 Medical Specializations

The system includes 37 medical specializations:

- Allergy and Immunology
- Anesthesiology
- Cardiology
- Cardiothoracic Surgery
- Dermatology
- Emergency Medicine
- Endocrinology
- Family Medicine
- Gastroenterology
- General Surgery
- Geriatrics
- Hematology
- Infectious Disease
- Internal Medicine
- Medical Genetics
- Nephrology
- Neurology
- Neurosurgery
- Nuclear Medicine
- Obstetrics and Gynecology
- Oncology
- Ophthalmology
- Orthopedic Surgery
- Otolaryngology (ENT)
- Pathology
- Pediatrics
- Physical Medicine and Rehabilitation
- Plastic Surgery
- Psychiatry
- Pulmonology
- Radiation Oncology
- Radiology
- Rheumatology
- Sports Medicine
- Thoracic Surgery
- Urology
- Vascular Surgery

## 🎯 Business Logic

### Doctor Approval Workflow
- Doctors register with `pending` status
- Admins can change status to `accepted` or `rejected`
- Only accepted doctors can receive consultation requests

### Consultation Request Flow
1. User sends consultation request to doctor (`pending`)
2. Doctor accepts or rejects request
3. If accepted, a chat is automatically created
4. Chat remains active until manually closed

### Messaging System
- Supports text, image, and file messages
- Messages are polymorphic (can be from users or doctors)
- File attachments stored as JSON for flexibility

### Notification System
- Polymorphic notifications for users, doctors, and admins
- Supports different notification types with JSON data storage
- Tracks read status and creation time
# Healthcare Consultation Platform


---
## 🛡️ Middleware Protection

### **Authentication Guards**
- `user.guard` - Protects user-specific routes
- `doctor.guard` - Protects doctor-specific routes  
- `admin.guard` - Protects admin-specific routes
- `auth:sanctum` - General API authentication

## 🛠️ Controllers & Models

### **Authentication Controllers**

#### UserAuthController
- `register()` - User registration with email verification
- `login()` - User email/password login
- `logout()` - User logout with token revocation
- `redirectToGoogle()` - OAuth Google redirect (Web)
- `handleGoogleCallback()` - OAuth Google callback (Web)
- `loginWithGoogle()` - OAuth Google login (Mobile)

#### DoctorAuthController
- `register()` - Doctor registration with clinic creation and specialization attachment
- `login()` - Doctor login with status validation
- `logout()` - Doctor logout

#### AdminAuthController
- `login()` - Admin login with email/name support
- `logout()` - Admin logout

#### EmailVerificationController
- `verify()` - Email verification endpoint

### **Business Logic Controllers**

#### UserController
- `profile()` - Get user profile
- `showAllSpecializations()` - List all medical specializations
- `doctorsBySpecialization()` - Get doctors filtered by specialization
- `doctorDetails()` - Get detailed doctor information
- `requestConsultation()` - Create consultation request
- `showAllReqeustsConsultation()` - Get user's consultation requests
- `userChats()` - Get user's chat sessions

#### DoctorController
- `profile()` - Get doctor profile with clinic and specializations
- `pendingConsultationRequests()` - Get pending consultation requests
- `respondToConsultation()` - Accept/reject consultation requests
- `closeChat()` - Close chat session
- `doctorChats()` - Get doctor's chat sessions

#### AdminController
- `createAdmin()` - Create new admin account
- `pendingDoctors()` - Get doctors pending approval
- `acceptDoctor()` - Approve doctor registration
- `rejectDoctor()` - Reject doctor registration
- `profile()` - Get admin profile

#### ChatController
- `sendMessage()` - Send message with file support
- `closeChat()` - Close chat session
- `getMessages()` - Retrieve chat messages with participant validation

### **Middleware**

#### Authentication Middleware
- `AuthenticateUser` - Validates user tokens and sets user context
- `AuthenticateDoctor` - Validates doctor tokens and sets doctor context  
- `AuthenticateAdmin` - Validates admin tokens and sets admin context
- `SetGuard` - Dynamically sets authentication guard

### **Models**

#### Core Models
- **User** - Authenticatable user with email verification
- **Doctor** - Authenticatable doctor with clinic relationship
- **Admin** - Authenticatable admin user

#### Domain Models
- **Specialization** - Medical specializations with doctor relationships
- **Clinic** - Healthcare clinics with location data
- **ConsultationRequest** - Consultation requests between users and doctors
- **Chat** - Chat sessions linked to consultations
- **Message** - Chat messages with polymorphic senders
- **Notification** - Polymorphic notifications system
- **DoctorSpecialization** - Pivot model for doctor-specialization relationships

### **Key Model Relationships**

```php
// User relationships
User::consultationRequests() → hasMany(ConsultationRequest::class)

// Doctor relationships  
Doctor::clinic() → belongsTo(Clinic::class)
Doctor::specializations() → belongsToMany(Specialization::class)
Doctor::consultationRequests() → hasMany(ConsultationRequest::class)

// ConsultationRequest relationships
ConsultationRequest::user() → belongsTo(User::class)
ConsultationRequest::doctor() → belongsTo(Doctor::class) 
ConsultationRequest::chat() → hasOne(Chat::class)

// Chat relationships
Chat::consultationRequest() → belongsTo(ConsultationRequest::class)
Chat::messages() → hasMany(Message::class)

// Message relationships (Polymorphic)
Message::sender() → morphTo()
## 🚀 Installation & Setup

```

---

## 🔄 Workflow Summary

### **User Journey**
1. **Register/Login** → Create account or sign in
2. **Verify Email** → Confirm email address for security
3. **Browse Specializations** → Explore medical specialties
4. **View Doctors** → See available healthcare providers
5. **Request Consultation** → Send consultation request to chosen doctor
6. **Chat** → Communicate with doctor in real-time

### **Doctor Journey**
1. **Register** → Create doctor account with credentials
2. **Wait for Admin Approval** → Account remains pending until approved
3. **Login** → Access platform after approval
4. **View Consultation Requests** → See pending consultation requests
5. **Accept/Reject** → Respond to patient requests
6. **Chat** → Engage in medical consultations with patients

### **Admin Journey**
1. **Login** → Access admin dashboard
2. **View Pending Doctors** → Review doctor registration requests
3. **Accept/Reject Doctors** → Approve or deny doctor applications
4. **Manage Platform** → Oversee platform operations and users
