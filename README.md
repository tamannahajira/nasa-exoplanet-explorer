# NASA Exoplanet Explorer

## Overview

NASA Exoplanet Explorer is a full-stack web application designed to simplify exploration of NASA's confirmed exoplanet dataset.

The platform allows users to search exoplanets using multiple discovery criteria, explore detailed planetary information, visualize discovery trends, and access official NASA resources from a unified interface.

The project focuses on efficient data retrieval and search performance by loading NASA's CSV dataset into memory and utilizing indexed search structures for rapid query execution.

---

## Features

### Search & Filtering

* Search exoplanets by Discovery Year
* Search by Discovery Method
* Search by Host Star
* Search by Discovery Facility
* Multi-filter query support
* Input validation
* Clear and reset functionality

### Results Table

* Dynamic result rendering
* Column sorting (ascending and descending)
* Pagination support
* Responsive table layout

### Planet Detail View

* Planet Name
* Host Star
* Discovery Information
* Planet Radius
* Planet Mass
* Orbital Period
* Distance Information
* NASA resource links
* Planet imagery with fallback placeholders

### Analytics Dashboard

* Total confirmed exoplanets
* Discovery method distribution
* Discovery facility statistics
* Discovery timeline visualization

### Performance Features

* Single-time CSV loading at application startup
* In-memory data caching
* Indexed search architecture
* Optimized query execution

---

## System Architecture

React Frontend
↓
REST API
↓
Node.js + Express Backend
↓
In-Memory Search Engine
↓
NASA Exoplanet Archive Dataset

The application loads NASA's CSV dataset during server initialization and builds searchable indexes for high-performance filtering operations.

---

## Tech Stack

### Frontend

* React
* Vite
* Axios
* Tailwind CSS
* Recharts

### Backend

* Node.js
* Express.js
* CSV Parser

### Deployment

* Vercel (Frontend)
* Render (Backend)

### Data Source

NASA Exoplanet Archive

---

## Search Optimization Strategy

Instead of scanning the entire dataset for every request, the application builds indexes during startup for:

* Discovery Year
* Discovery Method
* Host Star
* Discovery Facility

This approach significantly reduces query time and improves scalability as the dataset grows.

---

## Future Enhancements

* Automated NASA dataset synchronization
* Advanced filtering options
* Saved searches
* Planet comparison view
* User authentication
* Discovery prediction analytics
* Caching layer using Redis

---

## Getting Started

### Clone Repository

git clone <repository-url>

### Backend Setup

cd backend

npm install

npm start

### Frontend Setup

cd frontend

npm install

npm run dev

---

## Project Goals

This project was developed to demonstrate:

* Full Stack Development
* Data Engineering Concepts
* Search Optimization Techniques
* REST API Design
* Scientific Data Visualization
* Performance-Oriented Application Design

---

## License

This project uses publicly available data from NASA's Exoplanet Archive.

NASA remains the original source and owner of the dataset.

