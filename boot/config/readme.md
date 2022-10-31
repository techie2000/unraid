`.my_bash_*` and `.my_bashrc` files can (in theory) be used on any machine.

`.my_machine_*` files are really only designed for use on this system.

The `go` file appends the content of `.my_bash*` and `.my_machine*` file to the 'real' `.` files in `~/`

`.my_bashrc` >> `~/.bashrc`

`.my_bash_aliases` and `.my_machine_aliases` >> `~/.bash_aliases`
 
`.my_bash_functions` and `.my_machine_functions` >> `~/.bash_functions`
 
`.my_bash_prompt` >> `~/.bash_prompt`

`.my_bash_profile` >> `~/.bash_profile`




