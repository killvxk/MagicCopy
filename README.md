# MagicCopy
Powershell script to exfiltrate large files quickly and securely.

### MagicPut

Store file to a remote or local location.

'''
Magic-Put -PieceSize 10MB -File 'C:\MYBIGFILE.DATA' -Destination 'O:\' -Key "2U+lWBaZnQZHkMuYftz7TlM4h/9af+vXwWCPu7r3RcU="  -Threads 20 
'''

Recover lost pieces:

'''
Magic-Put -PieceSize 10MB -File 'C:\MYBIGFILE.DATA' -Destination 'O:\' -Key "2U+lWBaZnQZHkMuYftz7TlM4h/9af+vXwWCPu7r3RcU="  -FirstPiece 20 -LastPiece 25 
'''

### MagicGet

Recover file:

'''
Magic-Get  -File 'O:\MYBIGFILE.DATA' -Destination 'C:\' -Key "rJm0PP2KBhDoq87Q+hVqjwJt+NWguCRY1oLgRHmcSwY="
'''

### MagicGet

Recover file:

'''
Magic-Get  -File 'O:\MYBIGFILE.DATA' -Destination 'C:\' -Key "rJm0PP2KBhDoq87Q+hVqjwJt+NWguCRY1oLgRHmcSwY="
'''

### Generating Keys

'''
New-CryptographyKey -AsPlainText
''

