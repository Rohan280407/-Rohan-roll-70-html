# Veterinary Clinic Management System — Pet Owner Section

This module implements the **Pet Owner Section** for the **Veterinary Clinic Management System** web project using HTML5, CSS3, and vanilla JavaScript.

## Project Files

* **`petOwner.html`**: Main Pet Owner Portal page covering owner reviews, medical history records with dynamic row insertion and live search, a service cost estimator, diagnostic report upload with prescription status, and a link to `owner_new.html`.
* **`owner_new.html`**: Companion extra tools page providing a **Daily Feeding & Diet Schedule** list builder and a **Quick Care Feedback** form.
* **`prescribed-report.pdf`** *(optional sample asset)*: Target file linked from the prescription download prompt after a report upload.

## Features Overview

### 1. In `petOwner.html`
* **Pet Owner Reviews**: Displays review cards using `<img>`, `<blockquote>`, and `<q>` elements with sample dog and cat imagery.
* **Pet Medical History Table**: Displays owner name, pet name, weight, allergies, rabies vaccination status, and spayed/neutered status.
  * **Add New Pet Record (`addMedicalRow()`)**: Appends new rows to `<tbody>` using `insertRow()` and `insertCell()`, updates `#recordCount`, and clears the input fields.
  * **Live Search Filter (`searchTable()`)**: Filters rows dynamically as you type an owner or pet name into `#searchInput`.
* **Quick Service Cost Estimator (`calculateCost()`)**: Calculates and displays the estimated cost in INR (`₹`) for the selected veterinary service.
* **Upload Diagnostic Report & Prescription View (`handleUpload()`)**: Checks that `#ownerName` and `#reportFile` (`.jpg`, `.jpeg`, `.png`, `.pdf`) are provided, then reveals `#prescription-box` with the uploaded filename and prescription download link.
* **Link to Additional Pet Owner Tools**: Includes an anchor button (`<a href="owner_new.html" target="_blank" rel="noopener noreferrer">`) to open `owner_new.html`.

### 2. In `owner_new.html`
* **Daily Feeding & Diet Schedule (`addDietItem()`)**: Validates `#petDietName` and `#foodItem`, creates a new `<li>` entry with the chosen `#mealTime`, appends it to `#dietList`, and resets the text inputs.
* **Submit Quick Care Feedback (`saveFeedback()`)**: Validates `#ownerNote`, displays the selected `#ratingSelect` and note inside `#feedbackBox`, and clears the note textarea.

## How to Run & Test

1. Place `petOwner.html` and `owner_new.html` in the **same folder** so the link from `petOwner.html` to `owner_new.html` works properly.
   * *Code cleanup tip:* In `petOwner.html`, remove the outer duplicate `<!DOCTYPE html>` / `<html>` / `<body>` wrapper so there is only one clean HTML document structure per file.
2. **In VS Code**: Open the project folder and run `petOwner.html` using **Live Server** (or open it directly in a browser), then click **Additional Pet Owner Tools** to test `owner_new.html`.
3. **On Mobile**: Open the files in a mobile code editor or browser, or test each file in a web playground.
