# MSR606

A simple Python 3 application to read/write MSR cards using the msr606. Forked from https://github.com/xslim/msr606.

## Installation

- Clone this repository
- Python PIP should be pre-installed on your MacBook (see https://wiki.is.adyen.com/index.php/Python_PIP)
- Make sure you have the pySerial package (`pip3.4 install --index-url=https://pip.is.adyen.com pySerial --user`)

## Usage

- Reading: `./msr.py -d /dev/cu.usbserial -r`
- Writing: `./msr.py -d /dev/cu.usbserial -w -t 2 "PAN=YYMMSSS?"`

*NOTE:* While writing track 2: ommit the beginning `;` char

## Test Cards

### Payment cards

```
BCMC       67030010054610102=1808101?
CUP        6210947000000021=1808101?
JCB        3569990010082211=1808101?
Diners     36070500001376=1808101?
Discover   6510000000000166=1808101?
Amex       374245455400001=1808101?
Visa       4761739001010010=1808101?
Maestro    6799990200000001114=1808101?
Mastercard 5413330002001155=1808101?
```

### Gift cards

```
```
