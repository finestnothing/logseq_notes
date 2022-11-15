tags:: [[coding]], [[python]], [[syntax]]

- Decorator syntax is super powerful, and useful when there is a lot of code bein reused
	- Specifically when that code involves running functions
- It lets you run a function inside of another function
- ```python
  def function_wrapper (outer_function):
    def inner_function(*args, **kwargs):
      print("Inner_function start")
      for i in range(3):
        return_val = outer_function
      print("Inner_function end")
  
  @function_wrapper
  def outer_function():
    print("Outer Function")
    Return 1
    
  ```
	- Running outer_function() prints:
		- "Inner_function start"
		- "Outer Function"
		- "Outer Function"
		- "Outer Function"
		- "Inner_function end"
	- This is also useful for [[error_checking]] since you can make a single error_checking function, then throw the decorator syntax of it on all of your other functions