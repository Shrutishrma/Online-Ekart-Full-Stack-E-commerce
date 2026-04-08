# 🛒 SwiftCart: Full-Stack E-commerce CMS

**SwiftCart** (Online Ekart) is a complete online shopping ecosystem that handles everything from the moment a user browses a product to the final checkout. I built this to demonstrate how a modern storefront interacts with a secure, cloud-connected backend.

## 🚀 Key Features

* **Complete Shopping Flow:** Includes specialized components for Product Discovery, Category Filtering, Cart Management, and a multi-step Checkout process.
* **Cloud-Powered Media:** Utilizes **Cloudinary** and **Multer** to handle secure, high-resolution product image uploads and transformations.
* **Seamless Animations:** Leverages **Framer Motion** for fluid UI transitions and **Lucide React** for consistent, modern iconography.
* **Persistent Product Registry:** A robust **MySQL** backend managing product details, pricing, descriptions, and user feedback.
* **Responsive Styling:** Optimized for all devices using **Tailwind CSS** with a custom-configured design system.

## 🛠️ Technical Stack

| Layer | Technologies |
| :--- | :--- |
| **Frontend** | **React 18**, **React Router**, **Axios** |
| **Animation** | **Framer Motion**, **Lucide React** |
| **Backend** | **Node.js**, **Express** |
| **Database** | **MySQL** (via `mysql2` connection pooling) |
| **Storage** | **Cloudinary API** |

## 📂 Project Architecture

```text
SwiftCart/
├── backend/
│   ├── index.js            # Express server & Product API
│   └── package.json        # Backend dependencies
└── frontend/
    ├── src/
    │   ├── components/     # Cart, Checkout, ProductDetail, Category
    │   ├── pages/          # Main view containers
    │   └── App.jsx         # Navigation & State management
    └── tailwind.config.js  # UI design tokens
```

## 📡 API Endpoints (CMS)

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/dishes` | Retrieve the full product catalog |
| `POST` | `/create` | Upload image and add a new product |
| `PUT` | `/update/:id` | Update product details or images |
| `DELETE` | `/delete/:id` | Remove a product from the inventory |
| `POST` | `/feedback` | Process customer inquiries |

---
