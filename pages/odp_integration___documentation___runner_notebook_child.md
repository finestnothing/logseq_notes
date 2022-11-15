up:: [[odp_integration/documentation]]
alias:: odp_runner_notebook_child

- Purpose
	- This notebook is responsible for executing the step functions in the correct order
- inputs
	- integration_id
	- job_id
	- step_order
		- String order of steps to run
		- E.G. "get_df, write_df, upload_to_s3"
- variables
	- step_id_map
	  id:: 6372b136-dc79-47a9-8f3e-e9fdfe030909
		- A way of mapping step function names to an integer value
		- DONE get rid of this, exchange with just using the name of the function
	- global_param_dict
		- Holds variables for being passed between the [[odp_step_functions]]
			- params_df
				- dataframe of all parameters
			- param_map
				- dataframe of the parameter map table
			- step_id_map
				- ((6372b136-dc79-47a9-8f3e-e9fdfe030909))
			- DATABASE
				- defined constant for what database to use for accessing any tables
			- JOB_LOG_TABLE
				- table to be used for the job log level
			- STEP_LOG_TABLE
				- table to be used for the step log level
			- integration_id
			- job_id
- returns
	- "Success"
		- If no errors occur when running the step functions