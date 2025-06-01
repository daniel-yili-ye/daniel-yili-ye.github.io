+++
title = "Tabulate"
date = "2024-04-30"
tags = ["project", "web", "react", "nextjs", "ai", "vercel"]
draft = false
+++

**Effortlessly divide complex bills, including proportional taxes, tips, and discounts, among multiple payers—ensuring fair allocation every time, even with shared items!**

## Links
- **[🌐 Live Site](https://tabulate.vercel.app/)**
- **[💻 GitHub Repository](https://github.com/daniel-yili-ye/Tabulate)**

## Introduction

After countless experiences with manual calculations, [confusing spreadsheets](https://docs.google.com/spreadsheets/d/1ixzuB6UMTsaKO_n8LrY5zwVDDarukj9wdeHAAY13Cis/edit?usp=sharing), and clunky existing tools, I decided to build Tabulate, a solution designed to handle the vast majority (~80%) of typical bill-splitting scenarios with ease and accuracy.

## The Problem

Splitting bills, especially when some items are shared among different groups of people, can be tedious and prone to errors. Calculating everyone's fair share, including proportional tax and tip, often requires manual spreadsheets, which isn't always user-friendly, particularly for less tech-savvy individuals.

>"Isn't this just Splitwise?"

While Splitwise excels at managing shared expenses over time (like trips or roommate situations), it's not optimized for splitting individual bills with shared items and proportional costs. In Splitwise, individual bill split features are clunky to use or are paywalled (i.e. receipt OCR). Tabulate solves a specific use case where Splitwise falls short.[^1] Tabulate is purpose-built for those "in-the-moment" bill splits where you need to allocate shared items, tax, tip, and discounts accurately and proportionally. 

[^1]: Interestingly, Splitwise recognized this gap and created [Plates by Splitwise](https://plates.splitwise.com/), but it lacks key features like receipt OCR, custom tax/tip amounts, and a means to share your results. 

You can also use Tabulate as a compliment to Splitwise, by using Tabulate to calculate your bill split before entering it into Splitwise for a more longer-term expense tracking purpose.


**Common pain points:**
- Manual calculations are time-consuming and error-prone
- Existing tools often feel clunky or produce unexpected results
- Shared items are difficult to split fairly
- Proportional tax and tip calculations are complex
- Receipt scanning capabilities are often unreliable

## The Solution

Tabulate is a web-based bill-splitting tool that handles complex scenarios with ease:

1. **Smart Receipt Processing**: Upload a receipt image and let Google Gemini 2.0 automatically extract items and prices, or add items manually

2. **Flexible Item Assignment**: Assign entire items or portions to multiple people, with intuitive controls for shared items

3. **Automatic Calculations**: The app handles all the complex math:
   - Proportional tax and tip distribution based on each person's subtotal
   - Fair discount application across relevant items
   - Accurate cost splitting for shared items

4. **Clear Results**: Generate a detailed breakdown showing exactly what each person owes, with an option to create shareable links for easy communication

## Technology Stack

Built with modern web technologies for optimal performance and user experience:

- **Frontend**: Next.js (React) with TypeScript + Zod
- **Styling**: Tailwind CSS with Shadcn/ui components
- **Backend**: Supabase for data storage
- **AI Integration**: Google Gemini 2.0 for receipt scanning (OCR)
- **Deployment**: Vercel with analytics

## Impact & Future Plans

Tabulate has simplified bill-splitting for numerous group outings for myself and my friends. I've used it quite a bit while traveling to help me in split complex bills. For example, [here's](https://tabulate.vercel.app/bills/ed71fba1-a260-4109-91c5-9090b317ea1c) a complex bill split I made to figure out who owed what for a grocery trip during a recent trip to the Netherlands with friends (which was used to figure out WHAT exactly to enter into Splitwise for each person).

### Planned improvements:
- User accounts for saving bill history
- Support for multiple currencies
- More granular bill split options
    - by exact amounts
    - by percentages
    - by shares

## Key Learnings

This project provided valuable experience in:

- **AI Integration**: Working with Google Gemini 2.0 for practical OCR applications
- **Complex State Management**: Handling intricate bill-splitting logic with React, TypeScript, and Zod
- **User Experience Design**: Creating intuitive interfaces for complex financial calculations
- **Modern Web Development**: Implementing a full-stack solution with Next.js and Supabase