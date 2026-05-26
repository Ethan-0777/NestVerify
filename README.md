
# 馃彔 NestVerify 鈥� Rental House Finder with Verification System

> A web-based platform that connects tenants with verified rental properties, eliminating fake listings through a structured admin-controlled verification process.

---

## 馃搶 Table of Contents

- [About the Project](#about-the-project)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [System Modules](#system-modules)
- [Database Design](#database-design)
- [Verification System](#verification-system)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Screenshots](#screenshots)
- [Future Enhancements](#future-enhancements)
- [Author](#author)

---

## 馃摉 About the Project

**NestVerify** is a web-based Rental House Finder developed as a final-year BCA project. It addresses a common problem in the rental market 鈥� **fake and unverified property listings** 鈥� by introducing a document-based verification system managed by an admin.

House owners submit their property details along with identity and ownership documents. An admin reviews and approves only genuine listings, which then receive a **Verified** badge. Tenants can search and filter verified properties by location, budget, and facilities 鈥� making the rental process safer and more transparent.

---

## 鉁� Features

### 馃懁 User (Tenant)
- Register and log in securely
- Search rental properties using filters (location, budget, facilities)
- View verified property listings with detailed info
- Contact house owners directly

### 馃彙 Owner
- Register and upload property details (location, rent, facilities, images, contact)
- Submit identity proof and property documents for verification
- Track verification status of listed properties

### 馃洝锔� Admin
- Review submitted owner and property documents
- Approve or reject property listings
- Manage all users, owners, and property records

---

## 馃洜锔� Tech Stack

| Layer      | Technology                        |
|------------|-----------------------------------|
| Frontend   | HTML, CSS, JavaScript             |
| Backend    | PHP / Node.js / Python            |
| Database   | MySQL                             |
| Server     | XAMPP / Localhost                 |

---

## 馃З System Modules

```
NestVerify
鈹溾攢鈹€ User Module          鈫� Registration, login, property search
鈹溾攢鈹€ Owner Module         鈫� Property listing, document upload
鈹溾攢鈹€ Verification Module  鈫� Document review and approval flow
鈹溾攢鈹€ Search & Filter      鈫� Location, budget, and facility filters
鈹溾攢鈹€ Admin Module         鈫� Approval dashboard, user management
鈹斺攢鈹€ Database Module      鈫� Structured data storage and retrieval
```

---

## 馃梽锔� Database Design

The database is structured to avoid redundancy, maintain integrity, and allow fast retrieval.

| Table               | Purpose                                  |
|---------------------|------------------------------------------|
| `users`             | Stores tenant account information        |
| `owners`            | Stores house owner profiles              |
| `properties`        | Stores property listings and details     |
| `verification_details` | Stores submitted documents and status |
| `bookings`          | Stores contact/booking requests          |
| `admin_records`     | Stores admin actions and logs            |

---

## 鉁� Verification System

This is the **core feature** of NestVerify.

```
Owner uploads property details
        鈫�
Owner submits identity proof + property documents
        鈫�
Admin reviews submitted documents
        鈫�
Admin approves or rejects the listing
        鈫�
Approved property receives 鉁� Verified badge
```

**Benefits:**
- Reduces fraudulent listings
- Builds trust between tenants and owners
- Ensures only authentic properties are visible to users

---

## 馃殌 Getting Started

### Prerequisites
- XAMPP (or any local server with PHP & MySQL support)
- A modern web browser

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/your-username/nestverify.git

# 2. Move the project to your server's root directory
#    For XAMPP: move to /xampp/htdocs/nestverify

# 3. Import the database
#    Open phpMyAdmin 鈫� Create a new database 鈫� Import nestverify.sql

# 4. Configure database connection
#    Edit config/db.php (or equivalent) with your DB credentials

# 5. Start Apache and MySQL from XAMPP Control Panel

# 6. Open in browser
http://localhost/nestverify
```

---

## 馃搧 Project Structure

```
nestverify/
鈹溾攢鈹€ index.html / index.php       # Landing / Home page
鈹溾攢鈹€ register.php                 # User & Owner registration
鈹溾攢鈹€ login.php                    # Login page
鈹溾攢鈹€ search.php                   # Property search with filters
鈹溾攢鈹€ property-listing.php         # Property detail pages
鈹溾攢鈹€ verification-status.php      # Show verified/pending status
鈹溾攢鈹€ admin/
鈹�   鈹溾攢鈹€ dashboard.php            # Admin panel
鈹�   鈹溾攢鈹€ approve.php              # Document review & approval
鈹�   鈹斺攢鈹€ manage-users.php         # User/Owner management
鈹溾攢鈹€ assets/
鈹�   鈹溾攢鈹€ css/                     # Stylesheets
鈹�   鈹溾攢鈹€ js/                      # Scripts
鈹�   鈹斺攢鈹€ images/                  # UI and property images
鈹溾攢鈹€ uploads/                     # Owner-submitted documents
鈹溾攢鈹€ config/
鈹�   鈹斺攢鈹€ db.php                   # Database connection
鈹斺攢鈹€ nestverify.sql               # Database schema & sample data
```

---

## 馃摳 Screenshots

> _Add screenshots of your project here._

| Page | Preview |
|------|---------|
| Home Page | _(add screenshot)_ |
| Property Search | _(add screenshot)_ |
| Verified Listing | _(add screenshot)_ |
| Admin Dashboard | _(add screenshot)_ |

---

## 馃敭 Future Enhancements

- [ ] 馃 AI-based fake listing detection
- [ ] 馃搷 GPS / map-based location integration
- [ ] 馃挸 Online rent payment system
- [ ] 馃挰 Real-time chat between owner and tenant
- [ ] 馃摫 Mobile app version

---

## 馃懆鈥嶐煉� Author

**Nabin Raspeda**  
Roll Number: 2358BCA069  
Bachelor in Computer Application 鈥� Final Year  
Department of Computer Application  
MITS Institute of Professional Studies, Vikram Dev University  

Supervised by: **Ms. Laxmi Priya**  
Project Duration: April 2026 鈥� May 2026

---

## 馃搫 License

This project was developed for academic purposes.  
Feel free to use it as a reference for your own learning.

---

> 猸� If you found this project helpful, consider giving it a star on GitHub!
