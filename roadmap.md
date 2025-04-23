## 🧠 DASSTRINGS NOTE – DEVELOPMENT ROADMAP

---

### 📘 **Project Overview**

**Dasstrings Note** is a multi-tenant Progressive Web App (PWA) for managing lesson notes within educational institutions. It enables **teachers** to create structured lesson plans, **school admins** to review and approve them, and **super admins** to oversee all system activity across schools. The platform supports file uploads, real-time feedback, role-based access, and email notifications — all built with a modern full-stack JavaScript architecture.

---

### ✅ **Core Features**

#### 👤 User Roles
- **Super Admin**: Manages all schools, users, and system settings.
- **School Admin**: Manages school data, invites teachers, reviews notes.
- **Teacher**: Creates and submits weekly lesson notes, responds to feedback.

#### 📚 Lesson Note Workflow
- Teachers draft and submit structured notes weekly.
- Admins approve or reject notes with comments.
- Teachers revise and resubmit.
- Notes are archived after approval.

#### 📤 Uploads & Media
- PDF/Word file uploads (lesson notes)
- Image upload for user avatars (via Cloudinary)

#### 🔔 Notifications
- Email alerts for approvals, rejections, feedback, and reminders.

#### 🧾 Reporting
- Submission logs and downloadable report history for Admins.

#### ⚙️ System Capabilities
- Responsive UI across all screen sizes
- Offline-ready PWA support
- Role-based access control
- Email onboarding and invitation flow

---

### 💻 **Technology Stack**

| Layer             | Tool / Service                                                                 |
|------------------|----------------------------------------------------------------------------------|
| **Frontend**     | [Next.js 14](https://nextjs.org), [Tailwind CSS](https://tailwindcss.com), [ShadCN UI](https://ui.shadcn.com/docs/installation) |
| **Auth**         | [Auth0](https://auth0.com/docs) – Secure, scalable auth with roles and JWT |
| **Database**     | [MongoDB Atlas](https://www.mongodb.com/docs/atlas) – NoSQL document database |
| **ORM**          | [Prisma](https://www.prisma.io/docs) – MongoDB adapter with schema modeling |
| **File Uploads** | [UploadThing](https://uploadthing.com) – Handle PDFs, Word files, images |
| **Image Hosting**| [Cloudinary](https://cloudinary.com/documentation) – Fast optimized avatar serving |
| **Emails**       | [Nodemailer](https://nodemailer.com/about/) – SMTP email via Gmail or Outlook |
| **Hosting**      | [Vercel](https://vercel.com) – Seamless frontend + backend deployment |

---

### 🧱 **Development Phases & Milestones**

---

## 🚀 Phase 0 – Project Initialization

✅ Tasks:
- [ ] Create Next.js App (`npx create-next-app@latest`)
- [ ] Setup Tailwind CSS
- [ ] Install ShadCN UI
- [ ] Setup TypeScript, ESLint, Prettier
- [ ] Initialize Git repo + GitHub

---

## 🔐 Phase 1 – Authentication System

✅ Tasks:
- [ ] Configure Auth0 in Next.js project
- [ ] Protect routes using middleware
- [ ] Create login, signup, logout flow
- [ ] Auto-assign roles: SUPER_ADMIN, ADMIN, TEACHER
- [ ] Store Auth0 user profile in Prisma/MongoDB on first login
- [ ] Manual Super Admin seeding

---

## 🏫 Phase 2 – School & User Management

✅ Tasks:
- [ ] Create `schools` model
- [ ] Link `users` to `schoolId`
- [ ] Build School Admin dashboard
- [ ] Allow Admins to invite Teachers by email
- [ ] Build Teacher onboarding: first-login profile setup

---

## 📘 Phase 3 – Lesson Notes & Review System

✅ Tasks:
- [ ] Create `lesson_notes` model with fields (class, subject, week, objectives, fileUrl)
- [ ] Upload notes via [UploadThing](https://docs.uploadthing.com/)
- [ ] Admin can approve/reject with comments
- [ ] Feedback thread model per note
- [ ] Teachers can edit and resubmit rejected notes

---

## 👤 Phase 4 – Profile Management & Avatar Upload

✅ Tasks:
- [ ] Create user profile page
- [ ] Upload avatar with [Cloudinary](https://cloudinary.com/documentation/image_upload_api_reference)
- [ ] Default image fallback

---

## 📊 Phase 5 – Reporting & Admin Dashboard

✅ Tasks:
- [ ] Teacher dashboard: see all submissions + filters
- [ ] Admin dashboard: see all notes by status/date/class
- [ ] Export history to CSV (optional)

---

## ✉️ Phase 6 – Email Notifications

✅ Tasks:
- [ ] Integrate [Nodemailer](https://nodemailer.com/about/) with Gmail SMTP
- [ ] Notify Teachers:
  - Feedback received
  - Approval/Rejection
- [ ] Notify Admins on new submissions
- [ ] Optional: Scheduled weekly reminders

---

## 🌐 Phase 7 – PWA Features & Final Polish

✅ Tasks:
- [ ] Add [`next-pwa`](https://www.npmjs.com/package/next-pwa) plugin
- [ ] Create manifest, install prompt, favicon
- [ ] Offline caching for lesson drafts
- [ ] Mobile-first UI polish
- [ ] Accessibility: keyboard navigation, screen reader support

---

### 📚 Reference Docs

| Tool          | Docs |
|---------------|------|
| Next.js       | [https://nextjs.org/docs](https://nextjs.org/docs) |
| Prisma        | [https://www.prisma.io/docs](https://www.prisma.io/docs) |
| MongoDB       | [https://www.mongodb.com/docs/atlas](https://www.mongodb.com/docs/atlas) |
| Auth0         | [https://auth0.com/docs](https://auth0.com/docs) |
| Tailwind CSS  | [https://tailwindcss.com/docs](https://tailwindcss.com/docs) |
| ShadCN UI     | [https://ui.shadcn.com/docs/installation](https://ui.shadcn.com/docs/installation) |
| UploadThing   | [https://docs.uploadthing.com/](https://docs.uploadthing.com/) |
| Cloudinary    | [https://cloudinary.com/documentation](https://cloudinary.com/documentation) |
| Nodemailer    | [https://nodemailer.com/about/](https://nodemailer.com/about/) |

---