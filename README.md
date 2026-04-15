## Next.js Dashboard - Chapter 1: Getting Started
Welcome to the starter project for the Next.js Dashboard tutorial. This chapter covers setting up the project, exploring the folder structure, and running the development server.

## Installation
We recommend using pnpm as your package manager for its speed and efficiency.

1. Install pnpm (if not already installed)
npm install -g pnpm

2. Create the Project
Run the following command to set up the application using the official starter template:

      npx create-next-app@latest nextjs-dashboard \
      --example "https://github.com/vercel/next-learn/tree/main/dashboard/starter-example" \
      --use-pnpm

3. Setup and Run
Navigate into the project directory, install dependencies, and start the development server:

    cd nextjs-dashboard
    pnpm i
    pnpm dev
   
The app should now be running on http://localhost:3000.

## 📂 Project Structure
This project follows the Next.js App Router architecture. Here is a breakdown of the key directories:FolderPurpose/appContains all routes, components, and application logic./app/libContains reusable utility functions and data fetching logic./app/uiContains pre-styled UI components (cards, tables, forms)./publicStatic assets like images and icons.Config FilesRoot files like next.config.ts and tsconfig.json.

## 🛡️ TypeScript & Data

Placeholder DataTo help with UI development before a database is connected, placeholder data is provided in /app/lib/placeholder-data.ts.

TypeScript
const invoices = [
  {
    customer_id: customers[0].id,
    amount: 15795,
    status: 'pending',
    date: '2022-12-06',
  },
  // ...
];

## Type Definitions
This project is written in TypeScript. Type definitions are manually declared in /app/lib/definitions.ts to ensure data integrity across the application.
Example of the Invoice type:
TypeScript

export type Invoice = {
  id: string;
  customer_id: string;
  amount: number;
  date: string;
  status: 'pending' | 'paid'; // String union type
};

## 🚀 Key Features Explored
CLI Setup: Utilizing create-next-app for rapid scaffolding.
Example Integration: Working with existing codebases to reflect real-world development workflows.
Development Server: Using Hot Module Replacement (HMR) to see changes in real-time.Completed Chapter 1 of the Next.js Learning Path.

## Next.js App Router Course - Starter

This is the starter template for the Next.js App Router Course. It contains the starting code for the dashboard application.

For more information, see the [course curriculum](https://nextjs.org/learn) on the Next.js Website.
