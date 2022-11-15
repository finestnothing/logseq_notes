up:: [[odp_integration/documentation]]
alias:: odp_jobapiutils

- Purpose
	- This is a supporting file full of functions
	- They are regarding creating jobs for running [[odp_runner_notebook_parent]] notebooks
- submit_temp_job
	- inputs
		- notebook_path
			- Path of notebook to run
		- timeout in seconds
		- integration_id
		- job_id
		- cluster_info
		- step_order
	- variables
		- token
			- Identifier to run notebooks under
		- libraries (line 13)
			- Libraries to install for the job
		- run_name (line 41)
			- Name to give for the job run