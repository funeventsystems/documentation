# FES Ticket system.


## Introduction

Welcome to the documentation for our Ticket System! This system allows users to purchase, verify, and manage tickets for Masterminds shows. Whether you're an attendee or an administrator, this guide provides step-by-step instructions on using the various features of our ticket system.

## Table of Contents

1.  Installation
2.  Ticket Purchase
3.  Ticket Verification
4.  Admin Setup
5.  Ticket Lookup
6.  API Endpoints

## 1. Installation 

### Prerequisites

Before getting started, ensure that you have the following dependencies installed:

-   Node.js
-   NPM (Node Package Manager)

### Setup

1.  Clone the repository to your local machine.
   
    
    `git clone https://github.com/your/repository.git` 
    
2.  Install the required Node.js packages.
    
    
    `npm install` 
    
3.  Start the server.
    

    
    `npm start` 
    
    The server will run at `http://localhost:8000`.
    

## 2. Ticket Purchase 

To purchase tickets for a Masterminds show, follow these steps:

1.  Navigate to the ticket purchase page at `http://localhost:8000/request`.
2.  Fill out the ticket request form with your name, email, phone, and the number of tickets.
3.  Submit the form.
4. A member of the team with a predefined email will receive the request and handle it from there.
![Ticket Purchase](https://github.com/funeventsystems/documentation/blob/main/image.png?raw=true)

## 3. Ticket Verification 

To verify a ticket, follow these steps:

1.  Go to the ticket verification page at `http://localhost:8000/checkin`.
2.  Enter the ticket ID in the provided field and click the "Verify Ticket" button.
3.  The system will confirm if the ticket is valid or has already been used.

![Ticket Verification](https://github.com/funeventsystems/documentation/blob/main/Screenshot%202023-11-30%20195211.png?raw=true)

## 4. Admin Setup 

Admins can set up shows and manage ticket registrations. Here's how:

1.  Access the admin setup page at `http://localhost:8000/admin`.
2.  Select the show date, provide an email address, and specify the number of tickets.
3.  Click the "Setup Ticket" button to register the show and generate unique IDs.

![Admin Setup](https://github.com/funeventsystems/documentation/blob/main/Screenshot%202023-11-30%20195058.png?raw=true)

## 5. Ticket Lookup 

To look up ticket details, use the ticket lookup page at `http://localhost:8000/check`.

1.  Enter the ticket ID in the lookup form.
2.  Click the "Lookup" button to view ticket details.

![Ticket Lookup](https://github.com/funeventsystems/documentation/blob/main/Screenshot%202023-11-30%20195147.png?raw=true)


## 6. API Endpoints 
The ticket system exposes several API endpoints for programmatic access. Refer to the API documentation for detailed information.

-   `/api/tickets-html`: Retrieve a list of tickets in HTML format.
-   `/api/ticket/:ticketId`: Get details for a specific ticket.
-   `/api/registershow`: Register a new show and generate tickets.
