# nofail
Run the shell command until successful.

# Manual installation:
The preferred way of installation is to simply add the nofail script somewhere into your path (e.g. add the directory to your PATH environment or copy nofail into an existing included path like /usr/local/bin).

# Install via NPM:

```
npm install --global shell-nofail
```

# Usage
```
nofail [-h] [-?] [-s sleep] [-r max_retry] shell_command
	[-h] show this help
	[-?] show this help
	[-s sleep] Command failure retry interval. Default: 1
	[-r max_retry] Maximum number of retries. 0 is infinite retry. Default: 0
```

# Configuration completion
1. Install `bash-completion`
```
sudo apt install bash-completion
```

2. Modify profile
```
echo "complete -F _command nofail" >> ~/.bashrc
```

3. Use new configuration
```
source ~/.bashrc 
```

# License
Copyright Longhao.Chen. Licensed under MIT.
