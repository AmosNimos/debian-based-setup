# start by reading step 3 before starting

1.

# Add non free contribution, to have access to nvidea f*cking driver!
sed -i -e 's/deb-src http://deb.debian.org/debian/ buster main/deb-src http://deb.debian.org/debian/ buster main non-free contrib/g' /etc/apt/sources.list

# Install nvidia-detect

apt -y install nvidia-detect 

Or 

https://packages.debian.org/buster/amd64/nvidia-detect/download

2.

#Search for the driver suggested by nvidia-detect

nvidia-detect | sed -n '5p' | awk '{print "Install driver series: "$13"xx"}'

Or

nvidia-detect

# Install the deb file
https://www.nvidia.com/en-us/drivers/unix/

3.

# Give up
Download Ubuntu
