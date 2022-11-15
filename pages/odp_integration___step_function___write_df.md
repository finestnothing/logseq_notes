up:: [[odp_integration/documentation]]

- purpose
	- Write a dataframe to a location
	- Supports csv and xlsx
- inputs
	- global_param_dict
		- [[odp_integration/variable/basic_df]]
			- Dataframe to write, usually from [[odp_integration/step_function/get_df]]
- parameters
	- [[odp_integration/variable/file_path]]
		- File path to write dataframe to
	- [[odp_integration/variable/file_name]]
		- File name to create at the file path to write
	- [[odp_integration/variable/file_type]]
		- Supports xlsx and csv