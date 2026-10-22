# PROJECT REPORT
## Interactive Product Inventory & Analytics Dashboard

**Student Name:** ____________________  
**Roll Number:** ____________________  
**Class / Department:** ____________________  
**Subject:** JavaScript Programming  
**Submitted To:** ____________________  
**Date:** ____________________

## 1. Introduction
The Interactive Product Inventory & Analytics Dashboard is a JavaScript-based application used to manage a small list of products. It allows the user to add products, enter prices, search for items, classify products according to price, and calculate inventory statistics. It demonstrates core JavaScript programming concepts in one practical project.

## 2. Objectives
- To understand arrays and objects in JavaScript.
- To accept and validate user input.
- To use conditional statements and switch blocks.
- To apply loops and break/continue statements.
- To create regular functions and arrow functions.
- To calculate total inventory value, average price, tax, and discount.
- To display results in a simple interactive dashboard.

## 3. Software Requirements
- Operating system: Windows 10/11 or equivalent
- Browser: Google Chrome, Microsoft Edge, or another modern browser
- Languages: HTML, CSS, JavaScript
- Additional software: Not required

## 4. System Design
Product information is stored in an array named `inventory`. Each product is an object containing an ID, name, and price. JavaScript functions validate and process the information. HTML provides the user interface, while CSS styles the dashboard.

## 5. Implementation
1. **Data initialization:** The program starts with sample product objects in an array.
2. **Input handling:** The user enters a product name and price. The price is converted to a number using `Number()`.
3. **Validation:** `if...else` checks that the name is not empty and the price is a valid positive number.
4. **Category assignment:** Products costing up to ₹500 are Budget, products costing up to ₹2,000 are Standard, and products above ₹2,000 are Premium.
5. **Switch statement:** A `switch` block gives a description for each category.
6. **Loops and flow control:** Loops search the inventory; `continue` skips invalid entries and `break` stops a search after the specified match limit.
7. **Functions:** Regular and arrow functions calculate categories, totals, averages, and final prices.
8. **Analytics:** The dashboard displays the product count, inventory value, average price, and premium product count.
9. **Tax and discount:** The calculator applies the selected discount first and then calculates tax on the discounted subtotal.

## 6. Sample Output
Initial products:
- Notebook — ₹80 — Budget
- Water Bottle — ₹350 — Budget
- Keyboard — ₹1,200 — Standard
- Headphones — ₹2,500 — Premium

Initial total inventory value = ₹4,130.00  
Number of products = 4  
Average product price = ₹1,032.50  
Premium products = 1

For example, if tax is 18% and discount is 10% on all initial products:
- Subtotal = ₹4,130.00
- Discount = ₹413.00
- Amount after discount = ₹3,717.00
- Tax = ₹669.06
- Final total = ₹4,386.06

## 7. Testing
| Test | Input / Action | Expected result |
|---|---|---|
| Add valid product | Pen, ₹20 | Product is added as Budget |
| Empty name | Blank name | Validation message appears |
| Invalid price | 0 or negative number | Validation message appears |
| Standard product | Keyboard, ₹1,200 | Standard badge appears |
| Premium product | Headphones, ₹2,500 | Premium badge appears |
| Search | Enter “key” | Keyboard is found |
| Calculator | 18% tax and 10% discount | Subtotal, discount, tax, and final total display |
| Delete | Click Delete | Product is removed and analytics update |

## 8. Advantages
- Easy to use and understand.
- Gives instant inventory statistics.
- Demonstrates several JavaScript concepts in one application.
- Validates user input.
- Can run locally in a browser without installation.

## 9. Limitations
- Product data is not permanently saved.
- The project is designed for a small sample inventory.
- It does not use a database or user login.

## 10. Future Scope
The project can be improved by adding local storage or a database, product quantities, category filters, export to CSV, and user authentication.

## 11. Conclusion
The Interactive Product Inventory & Analytics Dashboard successfully demonstrates fundamental JavaScript concepts such as arrays, objects, input conversion, conditional statements, switch blocks, loops, functions, arrow functions, and scope. It also provides practical inventory and price analytics through an interactive interface.
