# 🗺️ Dastrings Note – Project Roadmap

**Start Date:** 2025-04-23  
**Project Type:** Progressive Web App (PWA)  
**Tech Stack:** Next.js 14, MongoDB, Prisma, NextAuth v5, ShadCN UI, UploadThing, Cloudinary, OneSignal

---

## ✅ Stage 0 – Setup & Scaffolding
- [ ] Initialize Next.js project with App Router
- [ ] Configure Tailwind CSS and ShadCN UI
- [ ] Connect Prisma to MongoDB
- [ ] Setup UploadThing for file uploads
- [ ] Setup Cloudinary for image uploads
- [ ] Configure NextAuth v5 (email/password auth)
- [ ] Create basic layout and navigation

---

## 🔐 Stage 1 – Authentication & Roles
- [ ] Define `users` model in Prisma
- [ ] Enable NextAuth JWT sessions with role-based access
- [ ] Add middleware protection for routes
- [ ] Create signup form (School Admins only)
- [ ] Super Admin account created manually (seed or console)
- [ ] Auto-create school when School Admin signs up

---

## 🏫 Stage 2 – School & User Management
- [ ] Create `schools` model and link to `users`
- [ ] Super Admin: manage schools and admins
- [ ] School Admin: invite Teachers by email
- [ ] Secure invite link flow for Teachers
- [ ] Teacher profile completion after invite

---

## 📘 Stage 3 – Lesson Notes & Feedback
- [ ] Create `lesson_notes` model
- [ ] Create `feedback_threads` model for comments
- [ ] Teacher can submit notes (UploadThing support)
- [ ] Admin can review and comment (approve/reject)
- [ ] Teachers can revise and resubmit
- [ ] Lock notes after approval

---

## 👤 Stage 4 – Profile & Media
- [ ] Users can update profile info
- [ ] Profile image upload via Cloudinary
- [ ] Auto-pull avatar from email if available

---

## 📊 Stage 5 – Dashboards & Logs
- [ ] Admin: view submission stats, filters
- [ ] Export submission history as CSV
- [ ] Teacher: see submission history & status

---

## 🔔 Stage 6 – Notifications
- [ ] Integrate OneSignal for push notifications
- [ ] Notify Teachers of feedback and reminders
- [ ] Notify Admins of new submissions
- [ ] Optional: email reminders via nodemailer

---

## 🚀 Stage 7 – PWA & Polish
- [ ] Add PWA support with `next-pwa`
- [ ] Offline support for drafts
- [ ] Manifest, icons, install prompt
- [ ] Responsive design polish
- [ ] Accessibility improvements

---

> 🎉 This roadmap helps you tackle development in small, focused stages. Track each checkbox in your GitHub project board or Notion workspace for maximum clarity.
