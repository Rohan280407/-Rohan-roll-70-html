# 🐾 Veterinary Clinic Management System — Pet Owner Portal

An interactive, responsive web portal designed for pet owners and clinic administrators to manage pet medical histories, view customer reviews, estimate service costs, and handle diagnostic report uploads seamlessly. 

Developed as part of the Web Programming and Design coursework at Lovely Professional University (LPU).

---

## 🚀 Key Features

1. **Pet Owner Reviews Section (`.reviews-box`)**
   - Displays customer testimonials and feedback cards with styled profile avatars (`dog.jpg`, `cat.jpg`).
   - Built using CSS Grid for a clean, responsive two-column layout.

2. **Interactive Pet Medical History Table**
   - **Live Search Filter:** Instantly filter records by Owner Name or Pet Name using real-time JavaScript event handling (`onkeyup`).
   - **Dynamic Counter Badge:** Automatically tracks and updates the total number of active patient records.
   - **Dynamic Record Addition:** Allows staff/users to append new pet entries (Owner Name, Pet Name, Weight, Allergies, Rabies Vaccination, and Spay/Neuter status) directly into the table without page reloads.

3. **Quick Service Cost Estimator**
   - Dynamic JavaScript calculation tool enabling users to select various veterinary services (Consultation, Vaccinations, Blood Tests, Surgery) and instantly compute estimated costs.

4. **Diagnostic Report Upload & Prescription Viewer**
   - Allows users to input owner names and attach previous medical reports (`.jpg`, `.jpeg`, `.png`, `.pdf`).
   - Instantly generates status notifications and provides a downloadable prescription report link.

---

## 🛠️ Technologies Used

* **HTML5:** Semantic structural layout and form components.
* **CSS3:** Advanced styling featuring CSS Grid, Flexbox, custom color variables, borders, and responsive card layouts.
* **JavaScript (ES6):** DOM manipulation, live search algorithms, dynamic table row insertion, and interactive calculators.

---

## 📂 Project Directory Structure

```text
veterinary-clinic-portal/
│
├── index.html              # Main HTML, CSS, and JavaScript source file
├── dog.jpg                 # Profile image for Bruno (Dog review)
├── cat.jpg                 # Profile image for Bella (Cat review)
└── prescribed-report.pdf   # Sample downloadable prescription report document