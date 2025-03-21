#def calculate_discount(price, discount_percent):
    """Calculates final price after applying a discount if it's 20% or higher."""
    if discount_percent >= 20:
        discount_amount = (discount_percent / 100) * price
        return price - discount_amount
    return price  # Return original price if discount is less than 20%

# Prompt user for input
original_price = float(input("Enter the original price: "))
discount_percent = float(input("Enter the discount percentage: "))

# Calculate final price
final_price = calculate_discount(original_price, discount_percent)

# Print result
if discount_percent >= 20:
    print(f"Discount applied! Final price: ${final_price:.2f}")
else:
    print(f"No discount applied. Final price: ${final_price:.2f}")
    Applying discount
   Enter the original price: 100
Enter the discount percentage: 25
Discount applied! Final price: $75.00
no discount
Enter the original price: 100
Enter the discount percentage: 10
No discount applied. Final price: $100.00
