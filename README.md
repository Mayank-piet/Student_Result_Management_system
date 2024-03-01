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
project-root<br>
│<br>
├── src<br>
│   ├── controller<br>
│   │   ├── routerController.ts<br>
│   │   │   └── Contains logic for handling RESTful API routes.<br>
│   │   └── utility.ts<br>
│   │       └── Contains utility functions used by routerController.<br>
│   ├── database<br>
│   │   └── connectivity.ts<br>
│   │       └── Contains logic for connecting to the PostgreSQL database.<br>
│   ├── interfaces<br>
│   │   ├── inventory.ts<br>
│   │   │   └── Defines TypeScript interfaces for inventory items.<br>
│   │   └── inventoryItem.js<br>
│   │       └── Defines the schema/structure of an inventory item.<br>
│   ├── routers<br>
│   │   └── indexRouter.ts<br>
│   │       └── Handles CRUD operations on the inventory.<br>
│   └── index.js<br>
│       └── Acts as the landing page of the website.<br>
│<br>
├── test<br>
│   ├── controllers<br>
│   │   └── utility.ts<br>
│   │       └── Contains logic to test functions with static/mock data.<br>
│   └── mockdata<br>
│       ├── testData.ts<br>
│       │   └── Contains static mock data to test CheckDataType function.<br>
│       ├── testData2.ts<br>
│       │   └── Contains static/mock data to test checkValidData function.<br>
│       └── testData3.ts<br>
│           └── Contains static/mock data to test allFieldPresent function.<br>
│<br>
├── .env<br>
├── package.json<br>
└── tsconfig.json<br>

</p>
