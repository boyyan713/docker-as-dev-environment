docker run -ti --name spacemacs \
 -e DISPLAY="unix$DISPLAY" \
 -e UNAME="yanboyang713" \
 -e UID="boyang" \
 -e TZ=<your_time_zone> \
 -v /tmp/.X11-unix:/tmp/.X11-unix:ro \
 -v /etc/localtime:/etc/localtime:ro \
 -v /etc/machine-id:/etc/machine-id:ro \
 -v /var/run/dbus:/var/run/dbus \
 -v <path_to_your_workspace>:/mnt/workspace \
 spacemacs/develop
