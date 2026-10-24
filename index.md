# Assignment 6.2 — Backgrounds, Borders & Display

## Objective

Create a webpage with three differently styled cards and demonstrate CSS backgrounds, borders, display properties, width, height, max-width, and rounded corners.

## 1. HTML Code (`index.html`)

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Assignment 6.2 - Card Designs</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <h1>Choose Your Plan</h1>
        <p>Find the plan that suits your needs.</p>
    </header>

    <main class="cards-container">

        <div class="card basic">
            <h2>Basic</h2>
            <p>Perfect for beginners who are just getting started.</p>
            <button>Get Started</button>
        </div>

        <div class="card standard">
            <h2>Standard</h2>
            <p>Great for users who need more features and flexibility.</p>
            <button>Choose Standard</button>
        </div>

        <div class="card premium">
            <h2>Premium</h2>
            <p>Best for users who want the complete experience.</p>
            <button>Go Premium</button>
        </div>

    </main>

    <section class="display-demo">
        <h2>CSS Display Properties</h2>

        <p>Block example:</p>
        <span class="block-example">This is a block element.</span>

        <p>Inline example:</p>
        <span class="inline-example">Inline One</span>
        <span class="inline-example">Inline Two</span>

        <p>Inline-block example:</p>
        <span class="inline-block-example">Inline-block One</span>
        <span class="inline-block-example">Inline-block Two</span>
    </section>

</body>
</html>
```

## 2. CSS Code (`style.css`)

```css
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    padding: 20px;
    font-family: Arial, sans-serif;
    background-color: #f3f4f6;
    color: #222;
}

header {
    text-align: center;
    margin-bottom: 30px;
}

.cards-container {
    display: flex;
    justify-content: center;
    align-items: stretch;
    flex-wrap: wrap;
    gap: 20px;
    max-width: 1100px;
    margin: 0 auto;
}

.card {
    width: 300px;
    max-width: 100%;
    min-height: 250px;
    padding: 25px;
    border: 2px solid;
    border-radius: 15px;
    text-align: center;
    background-color: white;
}

.card h2 {
    margin-top: 0;
}

.card p {
    line-height: 1.6;
}

.card button {
    display: inline-block;
    padding: 10px 18px;
    border: none;
    border-radius: 6px;
    color: white;
    cursor: pointer;
}

/* Basic card design */
.basic {
    background-color: #e8f2ff;
    border-color: #2878d0;
}

.basic button {
    background-color: #2878d0;
}

/* Standard card design */
.standard {
    background-color: #e8fff1;
    border-color: #239957;
}

.standard button {
    background-color: #239957;
}

/* Premium card design */
.premium {
    background-color: #fff0df;
    border-color: #d97706;
}

.premium button {
    background-color: #d97706;
}

/* Display property examples */
.display-demo {
    max-width: 900px;
    margin: 40px auto 0;
    padding: 20px;
    background-color: white;
    border: 1px solid #ccc;
    border-radius: 12px;
}

.block-example {
    display: block;
    width: 100%;
    max-width: 350px;
    padding: 12px;
    background-color: #dbeafe;
    border: 1px solid #2878d0;
    border-radius: 5px;
}

.inline-example {
    display: inline;
    background-color: #dcfce7;
    border: 1px solid #239957;
    padding: 5px;
}

.inline-block-example {
    display: inline-block;
    width: 150px;
    height: 60px;
    margin: 5px;
    padding: 10px;
    background-color: #ffedd5;
    border: 1px solid #d97706;
    border-radius: 5px;
    text-align: center;
}

/* Responsive layout */
@media (max-width: 600px) {
    body {
        padding: 12px;
    }

    .card {
        width: 100%;
    }
}
```

## 3. Requirements Completed

* Created three cards: Basic, Standard, and Premium.
* Added a title, description, and button to each card.
* Used distinct background colors and border colors.
* Applied `border-radius` for rounded corners.
* Demonstrated `display: block`, `display: inline`, and `display: inline-block`.
* Used `width`, `height`, and `max-width`.
* Added spacing using `padding`, `margin`, and `gap`.
* Added a responsive layout for smaller screens.

## 4. Testing

1. Open `index.html` in a browser.
2. Check that all three cards have different designs.
3. Confirm that every card contains a title, description, and button.
4. Observe how the block, inline, and inline-block examples behave.
5. Resize the browser to check the responsive layout.
6. Take a screenshot after verifying the webpage.

## Result

The webpage demonstrates three differently styled cards and practical examples of CSS backgrounds, borders, rounded corners, display properties, sizing, and responsive layout.

## Submission

* `Assignment-6.2.md`
* `index.html`
* `style.css`
* Screenshot of the completed webpage
*