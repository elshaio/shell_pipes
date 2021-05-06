# shell_script
Simple way to execute a pipe commands on linux.

# How to use it?
Just install it using:
```sh
pip install git+https://github.com/elshaio/shell_pipes.git
```
Then you can for example do:
```python
from shell_pipes import shell_pipes

response = shell_pipes.execute('ps aux | wc -l')

print(response)
```
And you will receive an array with one element with the number of processes on your computer, when you throw a command that will receive more than one line on response, you will receive an array with N elements corresponding to N lines of your response.

