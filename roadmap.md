# 🗺️ Dastrings Note – Development Roadmap

**Start Date:** 2025-04-23  
**Project Type:** Progressive Web App (PWA)  
**Stack:** [Next.js](https://nextjs.org), [Prisma](https://www.prisma.io/), [MongoDB](https://www.mongodb.com/), [NextAuth](https://next-auth.js.org/), [Tailwind CSS](https://tailwindcss.com/), [ShadCN UI](https://ui.shadcn.com/docs/installation), [UploadThing](https://uploadthing.com/), [Cloudinary](https://cloudinary.com/), [OneSignal](https://onesignal.com/)

---

## ✅ Stage 0 – Project Setup
- [ ] Create a new [Next.js](https://nextjs.org/docs) 14 project (App Router)
- [ ] Configure [Tailwind CSS](https://tailwindcss.com/docs/installation) and [ShadCN UI](https://ui.shadcn.com/docs/installation)
- [ ] Initialize [Prisma](https://www.prisma.io/docs/getting-started) with [MongoDB](https://www.mongodb.com/cloud/atlas)
- [ ] Setup [NextAuth v5](https://next-auth.js.org/getting-started/introduction) with email/password login
- [ ] Connect [UploadThing](https://docs.uploadthing.com/) for file uploads
- [ ] Setup [Cloudinary](https://cloudinary.com/documentation) for image hosting
- [ ] Connect [OneSignal](https://documentation.onesignal.com/docs/web-push-setup) for push notifications

---

## 🔐 Stage 1 – Authentication & Roles
- [ ] Create `users` model using Prisma with `role` and `schoolId`
- [ ] Protect routes with middleware using [NextAuth](https://next-auth.js.org/configuration/nextjs)
- [ ] Create public signup page for **School Admins**
- [ ] Build secure login + invite flow for **Teachers**
- [ ] Seed initial **Super Admin** (manually or via script)

---

## 🏫 Stage 2 – School & User Management
- [ ] Create `schools` model in Prisma and relate to `users`
- [ ] Allow School Admin to invite teachers by email
- [ ] Teachers complete their profiles on first login
- [ ] Super Admin dashboard: View/edit schools and user roles

---

## 📘 Stage 3 – Lesson Notes & Feedback
- [ ] Create `lesson_notes` model with fields: class, subject, week, objectives, file link
- [ ] Use [UploadThing](https://docs.uploadthing.com/) to upload note PDFs and images
- [ ] Admins can **approve** or **reject** notes
- [ ] Build `feedback_threads` model for 2-way commenting (chat-style)
- [ ] Teachers can revise and resubmit until approved

---

## 👤 Stage 4 – Profiles & Media
- [ ] Users can edit their name, password, and photo
- [ ] Upload and serve profile images with [Cloudinary](https://cloudinary.com/documentation/image_upload_api_reference)
- [ ] Pull initial avatar from email service if available

---

## 📊 Stage 5 – Dashboards & Logs
- [ ] School Admin dashboard with stats (approved, pending, rejected)
- [ ] Teachers dashboard with submission history and filters
- [ ] Export logs as CSV (optional)

---

## 🔔 Stage 6 – Notifications
- [ ] Integrate [OneSignal](https://documentation.onesignal.com/docs/web-push-setup) for push notifications
- [ ] Notify Teachers on submission status (approved/rejected)
- [ ] Notify Admins on new lesson note submissions
- [ ] (Optional) Add email-based reminders using [Nodemailer](https://nodemailer.com/about/)

---

## 🚀 Stage 7 – PWA & Final Polish
- [ ] Add PWA support using [`next-pwa`](https://www.npmjs.com/package/next-pwa)
- [ ] Setup web manifest, app icons, splash screen
- [ ] Enable offline support for drafts via localStorage or IndexedDB
- [ ] Mobile/responsive polish using [Tailwind](https://tailwindcss.com/docs/responsive-design)
- [ ] Add accessibility improvements (ARIA, keyboard nav)

---

## 📚 Reference Links

| Tool | Docs |
|------|------|
| Next.js | [https://nextjs.org/docs] |
| Prisma | [https://www.prisma.io/docs] |
| MongoDB Atlas | [https://www.mongodb.com/docs/atlas/] |
| NextAuth | [https://next-auth.js.org] |
| Tailwind CSS | [https://tailwindcss.com/docs] |
| ShadCN UI | [https://ui.shadcn.com/docs/installation] |
| UploadThing | [https://docs.uploadthing.com/] |
| Cloudinary | [https://cloudinary.com/documentation] |
| OneSignal | [https://documentation.onesignal.com] |

---

> ✨ Track progress in GitHub Projects, Notion, or Trello — and check off each stage as you build.  
> This roadmap is your master checklist to launch Dastrings Note successfully.

