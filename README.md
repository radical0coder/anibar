# Anibar

Logistics and freight management system built with Django.

## Overview

Anibar is a backend-focused web application designed for managing shipments, freight operations, and related logistics processes. The system handles complex shipment data including routes, parties, charges, manifests, and operational statuses.

The project emphasizes clean data modeling, business logic implementation, and administrative efficiency.

## Key Features

- Comprehensive shipment management (air, sea, and land modes)
- Custom reference number generation with transactional safety
- Support for Master and House documents (MAWB / HAWB)
- Management of related parties (clients, shippers, consignees, carriers, agents)
- Charge tracking and financial fields
- Manifest and invoice generation
- Priority system and operational status tracking
- Advanced Django admin interface with import/export capabilities

## Technical Highlights

- Complex relational data models with proper use of foreign keys and many-to-many relationships
- Custom `save()` logic for automatic reference generation and calculations
- Transaction-safe operations for critical business data
- Separation of concerns across multiple apps
- Custom user model and role-related entities
- Production-oriented configuration using environment variables
- Integration of `django-import-export` for administrative efficiency

## Tech Stack

- **Backend:** Python, Django
- **Database:** MySQL / SQLite
- **Admin:** Django Admin + django-admin-interface + import-export
- **Other:** python-decouple, Pillow

## Project Structure

anibar/
├── account/             # Custom user and related party models
├── shipment_module/     # Core shipment logic and business rules
├── config/              # Project settings and configuration
└── manage.py

## Purpose

This project demonstrates the ability to design and implement a domain-specific enterprise system with complex business rules, robust data modeling, and a focus on operational reliability — skills directly relevant to corporate backend and full-stack roles.
