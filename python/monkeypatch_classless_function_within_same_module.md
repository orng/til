#Monkeypatch a function within a module
The `globals()` function can be used to access the global variables within a module. It returns a dictionary with the names of the variables, such as function names as keys. 

To replace the myfunc function:
```
temp = globals()['myfunc']
globals()['myfunc'] = someotherfunc
globals()['myfunc'] = temp
```
