# rclone
docker image for rclone

http://rclone.org/

usage: 

first time: 
docker run --name rclone -it --rm alljoynsville/rclone bash

inside. run rclone config

from another shell, copy the config:
docker cp rclone:/root/.rclone.conf .

once config is set:
docker run --name rclone -it --rm -v `pwd`/.rclone.conf:/root/.rclone.conf alljoynsville/rclone sh -c "rclone copy myfile gdrive:target_dir"
