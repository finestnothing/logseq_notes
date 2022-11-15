up:: [[odp_integration/documentation]]
alias:: odp_runner_notebook_parent

- Purpose
	- The primary purpose of this function is to be a last-resort way to catch errors that get thrown by [[odp_runner_notebook_child]]
- Inputs to notebook
	- integration_id
	- job_id
	- step_order
	- timeout
		- How long to wait before the [[odp_runner_notebook_child]] times out on any given command
		- In number of seconds
	- notebook_path
		- Path to child notebook to run
- variables:
	- DATABASE
		- Cmd 4, line 13
		- What database to use for the job log
	- LOG_TABLE
		- Cmd 4, line 14
		- What table to use for logging data
	- log_columns
		- Name of columns in LOG_TABLE
- Related
	- [[odp_runner_notebook_child]]