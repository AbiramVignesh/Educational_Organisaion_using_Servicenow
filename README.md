| Date | November 2, 2025 |
| :--- | :--- |
| **Team ID** | F53C03230D9D3649CD4402B24FF15FEB |
| **project Name** | Educational organization using ServiceNow |

# Educational Organisation using ServiceNow

## Project Overview

This project is a custom **Educational Management System** built on the ServiceNow platform. Its primary goal is to solve the problems of slow, error-prone manual data entry by automating the key administrative processes of a school or college.

The final application provides a single, reliable, and user-friendly interface for administrators to manage the complete student lifecycle, from initial admission to final academic progress tracking.

---

## Key Features

* **Automated Admission Process:** A visual process flow guides users through the defined admission stages (e.g., "New," "In progress," "Joined," "Rejected").
* **Smart Form Automation:**
    * **Pincode Update:** Automatically populates the `City`, `Mandal`, and `District` fields on the admission form when a `Pincode` is entered.
    * **Auto-Populate:** Instantly fills in all student details (Name, Father's Name, etc.) on the progress form as soon as an `Admission Number` is selected.
* **Automatic Grade Calculator:**
    * **Total:** Instantly calculates the `Total` marks as a user enters marks for each subject.
    * **Percentage:** Automatically calculates the `Percentage` based on the total.
    * **Result:** Automatically determines a `Result` ("Pass" or "Fail") based on the percentage.
* **Data Integrity:** All calculation fields (`Total`, `Percentage`, `Result`) are **read-only** to prevent manual errors and ensure data is always accurate.
* **Structured Data Model:** Uses table inheritance (`Admission` table extends a `Salesforce` base table) to efficiently share common student data.
* **Unique ID Generation:** Automatically assigns a unique "Admin Number" (e.g., `SAL0000001`) to every new record.

---

## Technology Stack

* **Platform:** ServiceNow
* **Data Model:** Custom Tables (including Table Inheritance)
* **Business Logic:** Client Scripts (`onLoad`, `onChange`)
* **ServiceNow API:** `g_form` (GlideForm)
* **User Interface:** Form Design, Form Layout, and Process Flow
* **Configuration:** Number Maintenance, Update Sets

---

## Project Documentation

This repository contains all documentation for the project, organized by the standard software development lifecycle (SDLC) phases.

*
