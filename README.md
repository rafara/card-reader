# card-reader


to install serial:
pip3.4 install --index-url=[URL HERE] pySerial --user



trigger read:
./msr.py -d /dev/cu.usbserial -r

trigger write:
./msr.py -d /dev/cu.usbserial -w -t 2 "PAN=YYMMSSS?”

example:

./msr.py -d /dev/cu.usbserial -w -t 2 "PAN=67030010054610102=1808101?"


./msr.py -d /dev/cu.usbserial -w -t 2 "PAN=1=%6277201287475229^00000000^X?3="


./msr.py -d /dev/cu.usbserial -w -t 2 ";60514362659100004742?"
