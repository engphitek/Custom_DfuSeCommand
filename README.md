# Custom_DfuSeCommand
Modified version of DfuSeCommand to enable conversion from hex file to dfu file

Command usage

DfuSeCommand.exe [options] [Agrument][[options] [Agrument]...]

  -?                   (Show this help)
  -c                   (Connect to a DFU device )
     --de  device      : Number of the device target, by default 0
     --al  target      : Number of the alternate target, by default 0
  -u                   (Upload flash contents to a .dfu file )
     --fn  file_name   : full path name of the file
  -d                   (Download the content of a file into MCU flash)
     --v               : verify after download
     --o               : optimize; removes FFs data
     --fn  file_name   : full path name (.dfu file)
  -g                   (Generates a dfu file from the hex file )
  Usage Example: DfuSeCommand.exe -g path/file.hex -out path/file.dfu -Vid 0483 -Pid DF11
