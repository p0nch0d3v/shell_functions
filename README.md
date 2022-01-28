# Shell functions
These functions can be used like `docker` wrap for common CLI's, such as go, python, dotnet, node, etc.
 
They can be added to your shell, like `bash` or `zsh` just adding the following line in the `.bashrc` or `.zshrc`

```sh
source ${PATH_OF_THE_FUCNTIONS}/sh_functions/docker-functions
```

Example of use:
```sh
$ docker-go  
```
Output:
```sh
Docker Go
[docker pull golang]
Using default tag: latest
latest: Pulling from library/golang
Digest: sha256:301609ebecc0ec4cd3174294220a4d9c92aab9015b3a2958297d7663aac627a1
Status: Image is up to date for golang:latest
docker.io/library/golang:latest
[docker run --rm -it -v /~:/app --workdir /app golang bash ]
root@7752413adef1:/app#
```