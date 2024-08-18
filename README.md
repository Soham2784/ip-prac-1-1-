<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Customized T-Shirt Order Form</title>
</head>
<body>
    <h1>Order Your Customized T-Shirt</h1>
    <form action="/submit-order" method="post">
        <fieldset>
            <legend>T-Shirt Details</legend>

            <label for="tagline">Tagline on the Shirt:</label>
            <input type="text" id="tagline" name="tagline" placeholder="Enter your tagline" required><br><br>

            <label for="color">Color:</label>
            <select id="color" name="color" required>
                <option value="">Select color</option>
                <option value="white">White</option>
                <option value="black">Black</option>
                <option value="blue">Blue</option>
                <option value="red">Red</option>
                <option value="green">Green</option>
            </select><br><br>

            <label for="size">Size:</label>
            <select id="size" name="size" required>
                <option value="">Select size</option>
                <option value="s">Small</option>
                <option value="m">Medium</option>
                <option value="l">Large</option>
                <option value="xl">X-Large</option>
            </select><br><br>

            <label for="quantity">Quantity:</label>
            <input type="number" id="quantity" name="quantity" min="1" max="100" required><br><br>

            <label for="delivery_date">Delivery Date:</label>
            <input type="date" id="delivery_date" name="delivery_date" required><br><br>
        </fieldset>

        <fieldset>
            <legend>Delivery Details</legend>

            <label for="name">Customer's Name:</label>
            <input type="text" id="name" name="name" placeholder="Enter customer's name" required><br><br>

            <label for="address">Address:</label>
            <input type="text" id="address" name="address" placeholder="Enter address" required><br><br>

            <label for="email">Email:</label>
            <input type="email" id="email" name="email" placeholder="Enter email address" required><br><br>

            <label for="phone">Phone Number:</label>
            <input type="tel" id="phone" name="phone" placeholder="Enter phone number" pattern="[0-9]{10}" required><br><br>
        </fieldset>

        <fieldset>
            <legend>Additional Comments</legend>

            <label for="comments">Comments:</label>
            <textarea id="comments" name="comments" rows="4" cols="50" placeholder="Enter any additional comments or special instructions"></textarea><br><br>
        </fieldset>

        <input type="submit" value="Submit Order">
        <input type="reset" value="Reset Form">
    </form>
</body>
</html>
