## Update `vendor`

Download the embedded Win32 Version of Python 3.7.9 from (https://www.python.org/ftp/python/3.7.9/python-3.7.9-embed-win32.zip)[here] and copy the following files into `vendor`:

- `_queue.pyd`
- `_socket.pyd`
- `_ssl.pyd`
- `libcrypto-1_1.dll`
- `libssl-1_1.dll`
- `select.pyd`
- `unicodedata.pyd`

Then run update packages from pypi with `pip install -t vendor -r requirements.txt --upgrade`.

## Licenses

This project and all containing files, except for those in `vendor` are licensed under `GPL-3.0-or-later`.

- OpenSSL 1.1 is licensed under (licenses/OpenSSL-1_1)[the dual OpenSSL and SSLeay license]
- Python 3.7 is licensed under (licenses/Python37)[the Python License]

You can find licenses for python packages downloaded with `pip` in their respective `*.dist-info` directory.