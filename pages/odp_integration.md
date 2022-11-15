up:: [[work]] 
tags:: [[project]]

- ODP Integration project for work
- The idea behind this project is to create a modular tool for a wide variety of uses
- Uses
	- Exporting and sending data
	- Ingesting data (possibly)
	- Processing data
- It is composed of step functions that can be chained together
	- I won't make pages for each step function, but here are the core ones:
	  collapsed:: true
		- get_df
		- write_df
		- send_to_teams
		- write_to_s3
		- encrypt
		- log_data
- Takeaways and reusable ideas
  id:: 63726790-c2ff-4871-8b4d-df978939ca87
	- [[python/calling_functions_by_string]]
	- [[python/decorator_syntax]] for [[error_checking]]
	- [[python/dictionary_for_variable_passing]]
	- [[python/spark]] in [[databricks]]
	- [[databricks/file_system]]
- Documentation
	- [[odp_integration/documentation]]
- Todo List
	- [[odp_integration/todo]]