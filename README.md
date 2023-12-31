# Minishell

Your shell should: <br/>
• Display a prompt when waiting for a new command. <br/>
• Have a working history. <br/>
• Search and launch the right executable (based on the PATH variable or using a
relative or an absolute path). <br/>
• Not interpret unclosed quotes or special characters which are not required by the
subject such as \ (backslash) or ; (semicolon). <br/>
• Handle ’ (single quote) which should prevent the shell from interpreting the metacharacters in the quoted sequence. <br/>
• Handle " (double quote) which should prevent the shell from interpreting the metacharacters in the quoted sequence except for $ (dollar sign). <br/>
• Implement redirections: <br/>
◦ < should redirect input. <br/>
◦ > should redirect output. <br/>
◦ << should be given a delimiter, then read the input until a line containing the
delimiter is seen. However, it doesn’t have to update the history! <br/>
◦ >> should redirect output in append mode. <br/>
• Implement pipes (| character). The output of each command in the pipeline is
connected to the input of the next command via a pipe. <br/>
• Handle environment variables ($ followed by a sequence of characters) which
should expand to their values. <br/>
• Handle $? which should expand to the exit status of the most recently executed
foreground pipeline. <br/>
• Handle ctrl-C, ctrl-D and ctrl-\ which should behave like in bash. <br/>
• In interactive mode: <br/>
◦ ctrl-C displays a new prompt on a new line. <br/>
◦ ctrl-D exits the shell. <br/>
◦ ctrl-\ does nothing. <br/>
• Your shell must implement the following builtins: <br/>
◦ echo with option -n <br/>
◦ cd with only a relative or absolute path <br/>
◦ pwd with no options <br/>
◦ export with no options <br/>
◦ unset with no options <br/>
◦ env with no options or arguments <br/>
◦ exit with no options
