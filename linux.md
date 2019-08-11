# Find file
1. By name: 

    `find . -iname "some name"`

2. By content 

    `grep -rinw '/path/to/somewhere/' -e 'pattern'"`

    * -r or -R is recursive,
    * -n is line number, and
    * -w stands for match the whole word.
    * -l (lower-case L) can be added to just give the file name of matching files.
    * Along with these, --exclude, --include, --exclude-dir {dir1, dir2} flags could be used for efficient searching

# Tmux
## Working with sessions
1. `tmux` - start new session
2. `tmux new -s myname` - start new session with name myname
3. `tmux a`  #  (or at, or attach) - attach to a detached session
4.  `tmux a -t myname` - attach to a session with a particular name
5. `tmux ls` - list all sessions

## Inside a session
Prefix is Ctrl+B

1. `Prefix+c` - new window
2. `Prefix+n, Prefix+p` - next or previous window
3. `Prefix+,` - rename window
4. `Prefix+%` -vertically split window
5. `Prefix+"` - horizontally split window
6. `Prefix+Num` - switch to a window {num}
7. `Prefix+D` - detach from a session
8. `Prefix+$` - rename current session
9. `Prefix+arrow` - switch to different panes

# Docker
1. `docker images` - list all images
2. `docker ps --all` ` list all containers
3. `docker build . -t name:tag --network="host"` - build an image
4. `docker run --net=host --runtime=nvidia --cpus="1.5" -e   NVIDIA_VISIBLE_DEVICES=2,3 -it -v /your/disk:/docker_disk --name <name_of_container> <name_of_image>:<tag_of_image> `
6. `docker exec -it <container_name_or_id> bash` - connect to the container
7. `docker commit <container_name> new_image_name:new_image_tag` - commit container 

 


