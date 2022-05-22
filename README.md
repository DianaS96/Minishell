# Minishell :shell:	
Attempt to recode simple shell.<br>
Minishell manages to parse prompt, launch builtins and executables (ls, grep, wc, etc.) with arguments.

## Functional
* Redirections (`>`, `>>`, `<`, `<<`) and pipes (`|`) are implemented.
* Environment variables are handled. <br>
As in real bash single quotes prevent minishell from interpreting the metacharacters in the quoted sequence.<br>
Double quotes prevent minishell from interpreting the metacharacters in the quoted sequence except for $ (dollar sign).
* $? expands to the exit status of the most recently executed foreground pipeline.
* Signals are processed.<br>
Use Ctrl-C to display new prompt on new line, Ctrl-D to quit the program. Ctrl-\ does nothing.
* Implemented builtins:
  * echo with option -n <br>
  * cd with only a relative or absolute path <br>
  * pwd with no options <br>
  * export with no options <br>
  * unset with no options <br>
  * env with no options or arguments <br>
  * exit with no options <br>

<details>
  <summary>Click to see video</summary>
  
  > <video src="https://user-images.githubusercontent.com/81222865/169703494-f64163cb-7c68-423a-a8ec-de825d6c980d.mov" type="video/mp4" width="2rem" controls>
</video>)
</details>


## Usage
1. Create executable file using command **`make`**
2. Run the program (**`./minishell`**)

## Authors
* <a href="https://github.com/sslowpok">Alexey</a> (pipes, redirects, signals, builtins)
* <a href="https://github.com/DianaS96">Diana</a> (parser, builtins)
