# Platanos — Damm Smart Truck

**Platanos** is a hackathon prototype designed to improve last-mile logistics for Damm/DDI delivery operations.

The project connects two decisions that are usually planned separately:

1. **Route planning**
2. **Truck loading**

The goal is simple: help delivery drivers know not only where to go, but also how the truck should be loaded so that each stop is faster, easier, and more efficient.

> **Do not optimize only the route. Optimize the full delivery operation.**

---

## 🚚 What It Does

Platanos provides a driver-facing web platform where a Damm delivery driver can:

- log in to a driver portal,
- see assigned delivery routes,
- check customer time windows,
- view estimated route duration,
- inspect truck loading information,
- review 2D/3D loading plans,
- and receive operational recommendations.

The prototype focuses on making delivery execution easier for the driver and more predictable for the logistics team.

---

## 🧪 Demo Routes

The demo uses three sample routes:

| Route | Area | Customers | Order lines | Pieces |
|---|---|---:|---:|---:|
| DR0006 | Mollet | 23 | 197 | 489 |
| DR0017 | Mollet / Granollers | 24 | 265 | 672 |
| DR0038 | Granollers / Canovelles | 23 | 198 | 578 |

These routes are used to demonstrate:

- route sequencing,
- customer availability,
- truck capacity constraints,
- product grouping,
- loading recommendations,
- and operational KPIs.

---

## 🧠 Core Idea

In real delivery operations, the shortest route is not always the best route.

A good delivery plan must consider:

- driving time,
- unloading effort,
- product accessibility,
- customer time windows,
- truck capacity,
- returnables,
- and warehouse preparation.

If the first customers are loaded in an inaccessible part of the truck, the driver wastes time searching, moving products, and reorganizing the load during the route.

Platanos connects route planning and truck loading into one operational decision.

---

## 🖥️ Web Prototype

The web prototype includes:

- login screen for Damm/DDI drivers,
- dashboard with assigned routes,
- route detail pages,
- route KPIs,
- customer time windows,
- truck loading view,
- simplified 2D truck layout,
- operational alerts,
- and impact summary.

The interface is designed to be simple, professional, and suitable for a hackathon demo.

---

## 📦 Truck Loading Module

The loading module represents the truck as a simplified layout:

- 6 pallets,
- 12 rows,
- 6 columns,
- multiple height levels,
- product categories:
  - boxes,
  - barrels,
  - returnables,
  - other units.

The loading strategy prioritizes:

- keeping first stops accessible,
- grouping products by delivery sequence,
- reserving space for returnables,
- and reducing unnecessary movement inside the truck.

---

## 🗺️ Route Planning Module

The route module explores route sequencing using:

- customer locations,
- estimated travel time,
- customer time windows,
- service time,
- and operational constraints.

The project also explores the idea of grouping nearby establishments into a single truck stop when several businesses are close enough to be served from one parking point.

---

## 📊 Expected Impact

Platanos can help reduce:

- time spent searching for products,
- unnecessary movements inside the truck,
- failed deliveries due to timing issues,
- loading inefficiencies,
- and operational uncertainty.

Potential benefits:

- faster unloading,
- better driver experience,
- clearer warehouse preparation,
- improved handling of returnables,
- better visibility of truck capacity,
- and more realistic route execution.

---

## 🛠️ Built With

- Python
- pandas
- Plotly
- Google Colab
- Excel
- OpenStreetMap / Nominatim
- React
- TypeScript
- Vite
- Tailwind CSS
- shadcn/ui
- Manus.io
- GitHub

---

## 📁 Repository Structure

```text
platanos-damm-smart-truck/
│
├── README.md
├── .gitignore
│
├── web/
│   └── Web prototype generated with Manus
│
├── scripts/
│   ├── dammfaltamapa.py
│   └── mapes_rutes_parades.py
│
├── data/
│   └── README.md
│
└── docs/
    └── screenshots/
