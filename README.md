# 🍽️ Mini Canteen Billing System

A simple, beginner-friendly website for a college mini project. It shows a small canteen menu, lets the user choose food items and quantities, and calculates the bill automatically.

The website follows the same idea as the original **Java Mini Project** (Scanner input, switch-case food selection, price × quantity, and an invalid-choice message). The website is **not connected** to the Java program. The billing logic is written again in JavaScript, using the same menu and prices.

## Menu

| Item  | Price |
|-------|-------|
| ☕ Tea   | ₹10 |
| 🥞 Dosa  | ₹30 |
| 🥤 Juice | ₹20 |

**Formula:** `Total Bill = Item Price × Quantity`
**Example:** Dosa ₹30 × 3 = ₹90

## Technologies Used

- HTML5 – page structure
- CSS3 – styling and responsive layout
- JavaScript (plain) – menu selection, calculations, validation and printing

No frameworks, no backend, no database and no paid APIs.

## Features

- Three food cards (Tea, Dosa, Juice) with emoji, price, quantity selector and **Add to Bill** button
- Add multiple food items to one bill
- Increase, decrease or remove items in the bill table
- Automatic item total and grand total
- **Generate Bill** shows a neat bill summary with date and time
- **Clear Bill** starts a new order
- **Print Bill** prints only the bill summary
- Validation messages for:
  - empty quantity, decimals, zero or negative numbers
  - quantity above the limit (50 per item)
  - generating or printing an empty order
  - invalid food choice (the "default" case, like the Java program)
- Responsive design for mobile and desktop

## How the Website Matches the Java Program

| Java program | Website |
|--------------|---------|
| Display menu with `System.out.println` | Food cards on the page |
| `Scanner` reads choice and quantity | Buttons and quantity box |
| `switch(ch)` sets `price` | `getPrice()` function with `switch` in `script.js` |
| `default:` prints "Invalid choice" | Returns `-1` and shows an error message |
| `total = price * qty` | `item.price * line.qty` |
| `System.out.println("Total Bill = ...")` | Grand total and bill summary |

## File Structure

```
mini-canteen-billing-system/
├── index.html    # Page structure
├── style.css     # All styling and responsive design
├── script.js     # Menu, quantity, total, validation, bill, print
└── README.md     # Project documentation
```

## Run Locally

1. Download or clone the project and keep all four files in the **same folder**.
2. Double-click `index.html` to open it in any browser (Chrome, Edge, Firefox).
3. No installation or internet connection is needed.

## Upload to GitHub

1. Create a free account at [github.com](https://github.com) and sign in.
2. Click **New** (or **+ → New repository**).
3. Enter a name, for example `mini-canteen-billing-system`, choose **Public**, and click **Create repository**.
4. Click **uploading an existing file**.
5. Drag and drop all four files: `index.html`, `style.css`, `script.js`, `README.md`.
6. Click **Commit changes**.

## Deploy with GitHub Pages

1. Open your repository and click **Settings**.
2. Click **Pages** in the left menu.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Under **Branch**, select `main` and the `/ (root)` folder, then click **Save**.
5. Wait one or two minutes and refresh the page. Your link will look like:

```
https://your-username.github.io/mini-canteen-billing-system/
```

Share this link to show your project online.

## Demo Steps (for your presentation)

1. Show the menu and explain the three items.
2. Choose Dosa, set quantity to 3, and click **Add to Bill** (₹90).
3. Add Tea and Juice, and change quantities in the bill table.
4. Click **Generate Bill** to show the final bill.
5. Try quantity `0` or a decimal to show the validation message.
6. Click **Generate Bill** with an empty order to show the empty-order message.
7. Show **Print Bill** and **Clear Bill**.

## Presented By

Name: ____________________
Class / Roll No.: ____________________
