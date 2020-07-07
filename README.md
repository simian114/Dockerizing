### Dockerizing

-----
##### minishell

```
docker build -t minishell .
docker run -it minishell ./minishell
```
-----
##### Cub3D

```
docker build -t cub3d .
docker run --rm \
    --env="DISPLAY" \
    --env="QT_X11_NO_MITSHM=1" \
    --volume="/tmp/.X11-unix:/tmp/.X11-unix:rw" \
    --ipc host \
    cub3d
```
