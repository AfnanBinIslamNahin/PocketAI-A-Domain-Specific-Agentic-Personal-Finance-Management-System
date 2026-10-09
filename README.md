# PocketAI

**PocketAI — A Domain-Specific Agentic Personal Finance Management System**

PocketAI is an AI-powered personal finance web application designed to help users manage their daily income, expenses, budgets, savings, receipts, and financial activity through natural language, voice, and image-based interaction.

Unlike a general-purpose chatbot, PocketAI is specifically restricted to **personal finance management**. The AI assistant is designed to work only with the user's financial data and finance-related requests.

The main goal of PocketAI is simple:

> **Tell PocketAI what you spent, and PocketAI will organize, analyze, and help you understand your money.**

---

## Project Overview

Traditional expense tracking applications require users to manually enter transaction amounts, select categories, calculate budgets, and analyze spending patterns.

PocketAI aims to reduce this manual effort by introducing an AI-powered personal finance assistant.

Users will be able to enter financial information through:

- Natural language text
- Voice input
- Receipt or bill images
- Manual transaction entry

PocketAI will process the input, extract relevant financial information, organize transactions, update budgets, analyze spending patterns, and provide personalized financial insights.

---

# Core Objectives

PocketAI is being developed with the following objectives:

- Simplify personal expense tracking
- Reduce manual financial data entry
- Support natural language financial interactions
- Provide personalized spending insights
- Help users understand where their money is going
- Help users manage monthly budgets
- Analyze financial behavior
- Provide spending reduction suggestions based on user data
- Support receipt-based transaction extraction
- Maintain strict separation between different users' financial data
- Restrict the AI assistant to personal finance-related tasks only

---

# How PocketAI Works

The overall system workflow is:

```text
                    USER
                      │
          ┌───────────┼───────────┐
          │           │           │
        TEXT        VOICE       IMAGE
          │           │           │
          │        Speech       Receipt
          │        to Text      Analysis
          │           │           │
          └───────────┼───────────┘
                      │
                      ▼
              FINANCE RELEVANCE
                    CHECK
                      │
             ┌────────┴────────┐
             │                 │
        Finance Related    Non-Finance
             │                 │
             ▼                 ▼
       PocketAI Agent         Reject
             │
             ▼
        Finance Tools
             │
    ┌────────┼─────────┐
    │        │         │
Expense   Budget    Analytics
 Tools     Tools       Tools
    │        │         │
    └────────┼─────────┘
             │
             ▼
        User Database
             │
             ▼
    Personalized Analysis
             │
             ▼
           USER
```

---

# Public Website

Before creating an account, visitors will be able to explore the public PocketAI website.

The public section will include:

- Home
- Features
- How It Works
- About PocketAI
- Privacy
- Login
- Sign Up

Visitors will be able to understand what PocketAI does before creating an account.

---

# User Authentication

PocketAI will provide a secure authentication system.

New users will be able to:

```text
Sign Up
   ↓
Create Account
   ↓
Initial Setup
   ↓
Dashboard
```

Existing users will be able to:

```text
Login
  ↓
Authentication
  ↓
Personal Dashboard
```

Every PocketAI account will have its own isolated financial workspace.

A user will only be able to access their own:

- Transactions
- Income records
- Expenses
- Budgets
- Savings goals
- Receipts
- Financial insights
- Reports

User financial information must never be accessible by another user.

---

# Main Dashboard

After login, users will be redirected to their personal PocketAI dashboard.

The dashboard will provide a quick overview of their current financial situation.

## Financial Summary

The main dashboard will display:

- Total Income
- Total Expenses
- Available Balance
- Savings
- Monthly Budget Status

Example:

```text
-----------------------------------------
              PocketAI
-----------------------------------------

Total Income        ৳50,000

Total Expenses      ৳32,500

Available Balance   ৳17,500

Savings             ৳8,000

-----------------------------------------
```

---

# Smart Expense Entry

PocketAI will allow users to enter expenses using natural language.

Example:

```text
Ajke lunch e 350 taka ar bus vara 70 taka khoroch hoise.
```

PocketAI will automatically identify:

```text
Lunch
Category: Food
Amount: ৳350

Bus Fare
Category: Transport
Amount: ৳70
```

The user will review the result before confirming the transaction.

```text
AI Prediction
      ↓
User Review
      ↓
Confirm
      ↓
Save to Database
```

This confirmation step will help prevent incorrect financial information from being stored.

---

# Multilingual Support

PocketAI is planned to support:

- English
- Bengali
- Banglish text input

Example Bengali input:

```text
আজকে বাজার করেছি ১২০০ টাকার।
```

Example Banglish input:

```text
Ajke bazar korlam 1200 tk.
```

Example English input:

```text
I spent 1200 taka on groceries today.
```

All three inputs should create a similar financial transaction.

---

# Voice-Based Expense Entry

PocketAI will support voice-based financial interaction.

Users will be able to speak in Bengali or English.

Example:

```text
"আজকে দুপুরে খাবারের জন্য ৩০০ টাকা খরচ করেছি।"
```

The voice processing workflow will be:

```text
Voice
  ↓
Speech-to-Text
  ↓
PocketAI Agent
  ↓
Transaction Extraction
  ↓
User Confirmation
  ↓
Database
```

Voice recognition will use pretrained speech recognition technology.

---

# Receipt Scanner

Users will be able to upload receipts or bills.

PocketAI will analyze the receipt and attempt to extract:

- Merchant name
- Date
- Total amount
- Purchased items
- Expense category

Example:

```text
--------------------------------
Receipt Analysis
--------------------------------

Merchant:
ABC Restaurant

Date:
09 October 2026

Total:
৳850

Suggested Category:
Food & Dining

--------------------------------
```

The user must confirm the extracted information before the transaction is saved.

---

# Image Relevance Validation

PocketAI is not a general image analysis application.

Uploaded images will first be checked to determine whether they contain finance-related information.

Example valid images:

- Restaurant receipts
- Shopping bills
- Utility bills
- Payment receipts
- Purchase invoices

Example invalid images:

- Selfies
- Nature photographs
- Random screenshots
- Animals
- Personal photographs without financial information

If a user uploads an unrelated image, PocketAI will respond with a message similar to:

```text
No financial information was detected in this image.

Please upload a receipt, bill, invoice, or another finance-related image.
```

PocketAI will not attempt to generate financial information from unrelated images.

---

# Transactions

PocketAI will maintain a complete transaction history for every user.

Example:

| Date | Description | Category | Type | Amount |
|---|---|---|---|---:|
| Oct 09 | Lunch | Food | Expense | ৳350 |
| Oct 09 | Bus Fare | Transport | Expense | ৳70 |
| Oct 08 | Salary | Income | Income | ৳50,000 |
| Oct 07 | Electricity Bill | Utilities | Expense | ৳1,500 |

Users will be able to:

- Add transactions
- Edit transactions
- Delete transactions
- Search transactions
- Filter by category
- Filter by date
- Filter by income or expense

---

# Budget Management

Users will be able to create monthly category-based budgets.

Example:

| Category | Budget | Spent | Remaining |
|---|---:|---:|---:|
| Food | ৳6,000 | ৳4,800 | ৳1,200 |
| Transport | ৳3,000 | ৳1,900 | ৳1,100 |
| Shopping | ৳5,000 | ৳4,700 | ৳300 |

PocketAI will notify users when they approach or exceed a budget.

Example:

```text
You have used 80% of your monthly Food budget.
```

or:

```text
Your Shopping budget has been exceeded by ৳850.
```

Budget calculations will use deterministic backend logic rather than relying entirely on LLM-generated calculations.

---

# Financial Analytics

PocketAI will analyze user spending patterns.

The analytics section may include:

- Monthly expense trends
- Income vs expense comparison
- Category-wise spending
- Weekly spending patterns
- Month-to-month comparison
- Highest spending categories
- Spending changes over time

Example:

```text
Food          32%
Shopping      22%
Bills         18%
Transport     15%
Others        13%
```

---

# Personalized Financial Insights

PocketAI will provide user-specific financial insights based on actual transaction data.

Example:

```text
Your food spending increased by 18% compared with last month.
```

Another example:

```text
Your Shopping expenses increased significantly this month.

You spent ৳2,100 more on Shopping compared with the previous month.
```

These insights will be generated using verified database calculations combined with AI-generated explanations.

The LLM should not invent financial numbers.

---

# Smart Spending Suggestions

Users will be able to ask PocketAI questions such as:

```text
My expenses are getting too high.
How can I reduce my spending?
```

PocketAI will first analyze the user's real financial data.

Example analysis:

```text
Food spending: +21%

Shopping spending: +38%

Transportation: Stable

Bills: Stable
```

PocketAI can then provide personalized budgeting suggestions such as:

```text
Your Shopping and Food expenses increased the most this month.

You may consider setting a stricter Shopping budget and a weekly Food spending limit.
```

PocketAI will focus on:

- Spending management
- Budgeting
- Expense analysis
- Savings planning

PocketAI is not intended to provide regulated investment, trading, or loan recommendations.

---

# PocketAI Assistant

PocketAI will include a finance-only AI assistant.

Users may ask questions such as:

```text
How much did I spend on food this month?
```

```text
What was my highest expense category?
```

```text
Compare this month's spending with last month.
```

```text
How much money do I have remaining in my monthly budget?
```

```text
Where can I reduce my expenses?
```

```text
Show my latest transactions.
```

The AI agent will retrieve real user data using backend tools before answering.

---

# Domain-Restricted AI

PocketAI is not designed to behave like a general-purpose chatbot.

It will only handle personal finance-related requests.

Examples of supported topics:

- Expenses
- Income
- Budgets
- Savings
- Receipts
- Transactions
- Spending analysis
- Financial summaries
- Spending trends
- Financial planning based on available user data

Example unsupported request:

```text
Teach me Python.
```

PocketAI should respond:

```text
I can only assist with personal finance management,
expenses, budgets, transactions, savings, and related financial insights.
```

---

# Agentic AI Architecture

PocketAI will use an LLM-based agent together with controlled tools.

```text
                 PocketAI Agent
                       │
                       ▼
                      LLM
                       │
        ┌──────────────┼──────────────┐
        │              │              │
        ▼              ▼              ▼
 Transaction       Budget         Analytics
    Tool             Tool            Tool
        │              │              │
        ├──────────────┼──────────────┤
                       │
                       ▼
                  PostgreSQL
```

The LLM will be responsible for understanding user intent and selecting appropriate finance tools.

Actual financial calculations, validation, and database operations will be handled by backend services.

---

# AI Strategy

PocketAI does not require training a custom machine learning model during the initial development stage.

The initial system will use:

- Large Language Models
- AI Agents
- Tool Calling
- Pretrained Speech Recognition
- Pretrained OCR / Document Understanding
- Rule-Based Automation
- Database Analytics

Therefore, the project follows an **agentic AI application development approach** rather than a traditional dataset-training-model workflow.

---

# User Data Isolation

Each database record will be associated with an authenticated user.

Conceptually:

```text
User A
 ├── Transactions
 ├── Budgets
 ├── Savings
 ├── Receipts
 └── Insights


User B
 ├── Transactions
 ├── Budgets
 ├── Savings
 ├── Receipts
 └── Insights
```

User A must never be able to access User B's financial information.

Strict authorization checks will be implemented at the backend and database level.

---

# Privacy and Security

Because PocketAI processes personal financial information, privacy and security are core project requirements.

Planned security measures include:

- Secure user authentication
- Password hashing
- User-level data isolation
- Authorization checks
- Secure API endpoints
- Input validation
- Protected database access
- HTTPS in production
- Secure receipt handling
- Controlled AI tool permissions
- Financial action confirmation
- User data deletion options

The AI model will not be allowed to directly modify sensitive financial information without backend validation.

---

# Planned Dashboard Navigation

```text
PocketAI

├── Dashboard
├── Transactions
├── PocketAI Assistant
├── Receipt Scanner
├── Budgets
├── Analytics
├── Forecast
├── Savings Goals
├── Reports
├── Notifications
└── Settings
```

---

# Core Dashboard Components

The main dashboard is planned to include:

### Financial Overview

- Total Income
- Total Expenses
- Current Balance
- Savings

### Quick AI Entry

Users can quickly enter financial information through text.

### Spending Overview

A visual representation of monthly spending.

### Budget Progress

Shows how much of each budget has already been used.

### AI Insight

Displays important financial observations.

### Recent Transactions

Displays the latest financial activity.

### Ask PocketAI

Quick access to the personal finance AI assistant.

---

# Savings Goals

Users will be able to create savings goals.

Example:

```text
Goal:
New Laptop

Target:
৳120,000

Saved:
৳45,000

Progress:
37.5%
```

PocketAI may use the user's savings history to provide progress estimates.

Any future projection will be clearly presented as an estimate rather than a guaranteed outcome.

---

# Financial Reports

PocketAI may provide weekly and monthly financial reports.

Example report:

```text
Monthly Financial Summary

Income:
৳50,000

Expenses:
৳32,500

Savings:
৳17,500

Highest Spending Category:
Food

Budget Status:
Within Monthly Budget
```

Reports may later be exportable as PDF or other supported formats.

---

# Technology Stack

The initial technology stack may include:

## Frontend

- React.js or Next.js
- Tailwind CSS

## Backend

- Python
- FastAPI

## Database

- PostgreSQL

## AI

- LLM API
- Agentic AI
- Tool Calling
- Structured Outputs

## Voice

- Pretrained Speech-to-Text Model

## Receipt Processing

- OCR
- Pretrained Document Understanding Model

## Authentication

- JWT / Secure Authentication System

## Infrastructure

- Docker
- GitHub
- Cloud Deployment

---

# Development Roadmap

## Phase 1 — Core Platform

- [ ] Project setup
- [ ] Landing page
- [ ] About page
- [ ] User registration
- [ ] User login
- [ ] User dashboard
- [ ] PostgreSQL database
- [ ] User-specific data isolation

## Phase 2 — Finance Management

- [ ] Manual income entry
- [ ] Manual expense entry
- [ ] Transaction history
- [ ] Transaction editing
- [ ] Transaction deletion
- [ ] Expense categories
- [ ] Budget management
- [ ] Basic financial analytics

## Phase 3 — PocketAI Agent

- [ ] Finance-only LLM integration
- [ ] Domain restriction
- [ ] Structured transaction extraction
- [ ] Tool calling
- [ ] Finance relevance validation
- [ ] Database query tools
- [ ] AI-powered financial insights

## Phase 4 — Multimodal Input

- [ ] Bengali voice input
- [ ] English voice input
- [ ] Receipt image upload
- [ ] Receipt text extraction
- [ ] Receipt relevance validation
- [ ] Transaction confirmation workflow

## Phase 5 — Advanced Intelligence

- [ ] Personalized spending analysis
- [ ] Spending reduction suggestions
- [ ] Monthly comparison
- [ ] Savings goals
- [ ] Spending forecasting
- [ ] Unusual expense detection
- [ ] Weekly financial summary
- [ ] Monthly financial report

## Phase 6 — Production

- [ ] Docker
- [ ] API security
- [ ] HTTPS
- [ ] Rate limiting
- [ ] Logging
- [ ] Monitoring
- [ ] Cloud deployment
- [ ] Production testing

---

# Current Project Status

🚧 **PocketAI is currently under development.**

The project is being developed incrementally, starting with the core financial management platform and later introducing AI agent capabilities, receipt processing, voice input, analytics, and personalized financial insights.

---

# Project Vision

The long-term vision of PocketAI is to build a simple and intelligent personal finance assistant that allows users to manage their finances without dealing with complicated spreadsheets or manually organizing every transaction.

Instead of requiring users to constantly manage financial data themselves, PocketAI aims to allow users to simply communicate naturally:

```text
"I spent 300 taka on lunch today."
```

and let the system handle the organization.

PocketAI is being designed around one central idea:

> **Personal finance management should feel like having a conversation, not maintaining a spreadsheet.**

---

# Disclaimer

PocketAI is a personal finance management and budgeting application.

It is intended to help users organize expenses, understand spending patterns, manage budgets, and review their financial activity.

PocketAI is not intended to provide professional investment, legal, tax, lending, or regulated financial advice.

Users should independently verify important financial decisions.

---

# Author

**Afnan Bin Islam Nahin**

AI / Machine Learning / Software Development

---

## PocketAI

**Track smarter. Understand your spending. Take control of your money.**
