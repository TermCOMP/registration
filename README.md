# TermComp Registration

To register, you need to create a pull request for this repository. More specifically, to register for a certain $category, checkout the branch for the corresponding competition (e.g., the branch 2025 for termCOMP '25) and add a line to $category.txt. The content of the line must be the identifier of your Docker image on Docker Hub, so that it can directly be passed to "docker pull".

For example, there might be an entry like
```
loat/loat-termcomp:b60f5e
```
in `Integer_Transition_Systems.txt`.

If you also want to run with certification, just append ` cert` to that line. So
```
loat/loat-termcomp:b60f5e cert
```
means that the given container should run both in uncertified and certified mode. It is currently not possible to register for certified mode only.
