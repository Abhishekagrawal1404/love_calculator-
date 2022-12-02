
# Haikus for Codespaces

This is a quick node project template for demoing Codespaces. It is based on the [Azure node sample](https://github.com/Azure-Samples/nodejs-docs-hello-world). It's great!!!

Point your browser to [Quickstart for GitHub Codespaces](https://docs.github.com/en/codespaces/getting-started/quickstart) for a tour of using Codespaces with this repo.
# Function to calculate the love percentage
def love_calculator(name1, name2):
  # Convert the names to lowercase
  name1 = name1.lower()
  name2 = name2.lower()

  # Remove all the whitespace from the names
  name1 = name1.replace(" ", "")
  name2 = name2.replace(" ", "")

  # Calculate the score by summing the ASCII values of the letters in the names
  score = 0
  for char in name1:
    score += ord(char)
  for char in name2:
    score += ord(char)

  # Calculate the love percentage
  love_percentage = score % 100

  return love_percentage

# Get the names from the user
name1 = input("Enter the first name: ")
name2 = input("Enter the second name: ")

# Calculate the love percentage and print the result
love_percentage = love_calculator(name1, name2)
print("The love percentage between", name1, "and", name2, "is", love_percentage, "%")
