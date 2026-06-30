# CS-340 — Animal Shelter Database & Dashboard

A full-stack data application built for a fictional client, Grazioso Salvare, to manage and visualize animal shelter records. The project pairs a Python CRUD module with a MongoDB backend and an interactive Jupyter dashboard for data exploration.

## Features
- **Custom CRUD Module** — A reusable `AnimalShelter` Python class providing create, read, update, and delete operations against a MongoDB collection, with built-in error handling and input validation
- **Interactive Dashboard** — A Jupyter Notebook dashboard that connects to the CRUD module to query, filter, and visualize shelter animal data in real time
- **Reusable Design** — The CRUD module is decoupled from the dashboard, allowing it to be reused across other applications or client requirements without modification

## Technical Overview
- **Backend:** Python, PyMongo, MongoDB
- **Frontend/Visualization:** Jupyter Notebook (interactive dashboard)
- **Architecture:** The CRUD module exposes a simple, consistent interface (`create`, `read`, `update`, `delete`) that abstracts away direct database queries, making the dashboard layer simpler to build and easier to maintain

## Design Approach
The project was split into two phases. The first focused on building a robust, reusable CRUD module independent of any specific UI. The second connected that module to a dashboard, allowing shelter data to be filtered and visualized without touching the underlying database logic directly. This separation of concerns made the codebase easier to test, debug, and extend, the same module could be reused for a different client or dataset with minimal changes.

## Setup Note
Database credentials are not hardcoded in this repository. To run this project locally, set the following environment variables before starting:
```
MONGO_USER, MONGO_PASS, MONGO_HOST, MONGO_PORT, MONGO_DB
```

## Tech Stack
Python, PyMongo, MongoDB, Jupyter Notebook
