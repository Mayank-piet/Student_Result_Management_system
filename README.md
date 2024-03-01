# Student_Result_Management_system

# Inventory Management System

Welcome to our amazing project, the Inventory Management System!

This system facilitates the management of inventory by accepting the following information:

- Name of the product
- Price of the product
  - Item Price (Integer)
  - Item Currency (Currently accepting INR, USD, YEN, and EURO)
- Quantity of the item to be added in inventory
- The person who is adding the item
- The timezone of the country where the person stays

## API Endpoints

The project provides 5 RESTful API endpoints to perform CRUD operations on the inventory:

1. GET /items: Retrieve all the items present inside the inventory.
2. GET /items/id: Retrieve a specific item with the given id from the inventory.
3. POST /items: Add an item into the inventory.
4. PATCH /items/id: Update an existing item with the given id in the inventory.
5. DELETE /items/id: Delete an existing item with the given id from the inventory.

<p>
project-root
│
├── src
│   ├── controller
│   │   ├── routerController.ts
│   │   │   └── Contains logic for handling RESTful API routes.
│   │   └── utility.ts
│   │       └── Contains utility functions used by routerController.
│   ├── database
│   │   └── connectivity.ts
│   │       └── Contains logic for connecting to the PostgreSQL database.
│   ├── interfaces
│   │   ├── inventory.ts
│   │   │   └── Defines TypeScript interfaces for inventory items.
│   │   └── inventoryItem.js
│   │       └── Defines the schema/structure of an inventory item.
│   ├── routers
│   │   └── indexRouter.ts
│   │       └── Handles CRUD operations on the inventory.
│   └── index.js
│       └── Acts as the landing page of the website.
│
├── test
│   ├── controllers
│   │   └── utility.ts
│   │       └── Contains logic to test functions with static/mock data.
│   └── mockdata
│       ├── testData.ts
│       │   └── Contains static mock data to test CheckDataType function.
│       ├── testData2.ts
│       │   └── Contains static/mock data to test checkValidData function.
│       └── testData3.ts
│           └── Contains static/mock data to test allFieldPresent function.
│
├── .env
├── package.json
└── tsconfig.json

</p>
