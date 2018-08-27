#!/bin/env python

import socket, os

s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
s.bind((socket.gethostname(), 9000))
s.listen(1)

while True:
    c, _ = s.accept()
    c.recv(128)
    os.system('bin/repo sync')
    c.close()
