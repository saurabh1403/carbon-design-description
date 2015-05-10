# Introduction #
the protocol to store any AES key into a character stream.
Add your content here.


# Details #

Key stream protocol

first three bytes:
a1a2a3 : denotes the algorithm type

next three bytes:
k1k2k3 : denotes the length of key. This length is the encoded key length and not the original one which can be lesser than the encoded one.

next three bytes:
i1i2i3 : denotes the length of iv vector. This length is the encoded iv length and not the original one which can be lesser than the encoded one.

next key block:
the key stored in base64 format

next iv block:
the iv stored in base64 format


