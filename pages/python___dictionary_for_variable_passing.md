tags:: #coding, #python, #coding/design

- This was an idea used in [[odp_integration]] for passing variables between related functions
- ```python
  variables = {
    "var1": val1,
    "var2": val2
  }
  
  def func1(variables):
    variables["var3"] = variables["var1"] + variables["var2"]
  def func2(variables):
    print(variables["var3"])
  
  func1(variables)
  func2(variables)
  ```
- The idea behind this is that it's modular variables
- You don't need to change the inputs of the function since you're only passing in the dictionary
	- You can access any variables in that dictionary by name
	- Can add, remove, or change any of the values
	- Useful for a modular system like [[odp_integration]] where your function order changes