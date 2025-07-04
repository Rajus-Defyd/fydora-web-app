
# fydora-web-app 

A responsive **doctor-side dashboard** of a healthcare platform, built using **Next.js (App Router)** and **Tailwind CSS**. This frontend application allows doctors to manage their appointments, view patient details, update their profiles, and more.

---

##  Project Overview

This project is focused on building the **frontend only** of a doctor-specific healthcare dashboard. The app is built using **Next.js with the App Router** and includes pages and components that simulate a working environment for doctors within a digital healthcare platform.


---

##  Tech Stack

| Layer         | Technology              |
|---------------|--------------------------|
| Framework     | Next.js (App Router)     |
| Styling       | Tailwind CSS]            |
| UI Components | Custom React Components  |
| Icons         | Lucide Icons             |
| Deployment    | Vercel                   |  
  
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

##  Theme Toggle

Dark mode is enabled using Tailwind’s `dark:` classes.  
```js

const toggleTheme = () => {
  document.documentElement.classList.toggle('dark');
};
