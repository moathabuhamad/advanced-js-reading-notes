# API Integration

## Dynamic API Server

An Express/Node.js based server designed to be a “model agnostic” REST API server, which can perform CRUD operations on any data model.

Support all REST/HTTP methods

GET: Retrieve record(s) from a data source
POST: Create a new record in a data source
PUT: Update a single full record in a data source
PATCH: Update part of a single record in a data source
DELETE: Delete a record in a data source

## Development Process, Milestones
Phase 1: API Basics

Use JSON Server (non-express) to mock the routes for testing purposes
Phase 2:

Basic API Create CRUD/ReST endpoints for categories and products

Separate route modules for each data model type

Store user created data in memory (no persistence)

Integrates with an online CI framework

Phase 3: Persistence

Replace the in-memory data store with mongo
Use Mongo Collections for each data model type
Phase 4: Dynamic Models

Create a single model class that all data models can inherit from to keep the interface simple
Use middleware to load models based on param i.e. Replace app.get('/api/v1/categories') and app.get('/api/v1/products') with app.get('/api/v1/:model')