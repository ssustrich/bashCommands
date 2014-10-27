Find size of file of type XXX in folder LOCATION\n
find LOCATION -type f -name "*.XXX" -exec du -shc {} + | tail -1 | awk '{print $1}'
