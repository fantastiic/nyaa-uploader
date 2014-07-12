Requires PyYaml and requests.

Fill in the blanks in creds.yaml.example and remove the .example

Keep the file in the same dir as the script, whatever that is.

It should just do what it says on the tin, if a bit rigidly.

usage: nyaa-uploader.py [-h] [-v] [-c CRC] [-g GROUP] [-t TITLE] [-p PART]
                        [-y TYPE] [-H] [-o] (-V VIDEO | -l) [-T TORRENT]
                        {lraw,lsub,araw,asub}

positional arguments:
  {lraw,lsub,araw,asub}
                        Nyaa/Tosho Category

optional arguments:
  -h, --help            show this help message and exit
  -v, --verbose         Print more data to stdout.
  -c CRC, --crc CRC     Override detected CRC
  -g GROUP, --group GROUP
                        Nyaa Group Field
  -t TITLE, --title TITLE
                        Nyaa Title Field
  -p PART, --part PART  Nyaa Part Field
  -y TYPE, --type TYPE  Nyaa Type Field
  -H, --hidden          Set Hidden on Nyaa?
  -o, --tosho           Submit torrent to tokyotosho.
  -V VIDEO, --video VIDEO
                        Video file torrent is named for.
  -l, --local           Use video/torrent in calling directory. Must be
                        exactly one.
  -T TORRENT, --torrent TORRENT
                        Torrent file, if it doesn't match video.
