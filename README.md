
# fydora-web-app – Frontend (Next.js)

A responsive and modern frontend web application for a healthcare platform, built using **Next.js** and **Tailwind CSS**. This app provides patients with an intuitive interface to manage their appointments, view health records, update profile information, and more.

---

##  Project Overview

This project focuses on building only the **frontend** of a healthcare web application using the **Next.js App Router**. It includes pages and components that simulate a real-world healthcare platform for patients.

---

##  Tech Stack

| Layer         | Technology              |
|---------------|--------------------------|
| Framework     | [Next.js (App Router)](https://nextjs.org/) |
| Styling       | [Tailwind CSS](https://tailwindcss.com/) |
| UI Components | Custom React Components |
| Icons         | [Lucide Icons](https://lucide.dev/)  |
| Deployment    | [Vercel](https://vercel.com/) |

---

##  Folder Structure

/app
├── layout.tsx # Global layout with Header/Footer  
├── page.tsx # Home page  
├── login/page.tsx  
├── signup/page.tsx  
├── dashboard/page.tsx  
├── appointments/page.tsx  
├── health-records/page.tsx  
├── profile/page.tsx  
├── contact/page.tsx  
├── feedback/page.tsx  
├── not-found.tsx # Custom 404  

/components  
├── Header.tsx  
├── Footer.tsx  
├── Sidebar.tsx  
├── ThemeToggle.tsx  
├── AppointmentCard.tsx  
├── PatientCard.tsx   

/styles  
├── globals.css  
├── tailwind.config.js  

/public   
├── /assets (images, logos)  
---

##  Pages


| Route               | Description                                |
|---------------------|--------------------------------------------|
| `/dashboard`        | Overview of appointments, patients         |
| `/appointments`     | View, confirm, or cancel appointments      |
| `/patients`         | View patient details and history (mock)    |
| `/profile`          | Edit doctor's name, specialization, etc.   |
| `/settings`         | Theme toggle, notification preferences     |
| `/not-found`        | Custom 404 page                            |

---

##  Reusable Components

| Component         | Purpose |
|------------------|---------|
| `Header`         | Top navigation bar |
| `Sidebar`        | Navigation panel (Dashboard, Patients, Settings, etc.) |
| `Footer`         | Footer with copyright |
| `ThemeToggle`    | Switch between dark/light modes |
| `AppointmentCard`| Card displaying appointment data |
| `PatientCard`    | Patient information in list/grid view |


---

##  Styling & Responsiveness

- Built with **Tailwind CSS**
- Fully responsive layout (mobile-first)
- Accessible UI with proper HTML semantics
- Consistent theming with custom color palette
- Smooth transitions and animations

---

##  Theme Toggle

Dark mode is enabled using Tailwind’s `dark:` classes.  
```js

const toggleTheme = () => {
  document.documentElement.classList.toggle('dark');
};
