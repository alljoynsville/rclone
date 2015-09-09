# rclone
docker image for rclone

http://rclone.org/

usage: 
first time: 
docker run -it --rm -v `pwd`:/root/ alljoynsville/rclone sh -c "rclone config"

once config is set:
docker run -it --rm -v `pwd`/.rclone.conf:/root/.rclone.conf alljoynsville/rclone sh -c "rclone copy myfile gdrive:target_dir"
.rclone.conf

