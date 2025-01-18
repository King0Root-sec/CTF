# CYSSSA-CTF

Yoo man, it my first time doing a write up for a ctf but let dive in 

Warm up

![image](https://github.com/user-attachments/assets/2e6ebe0d-d2d7-48a4-bcf5-1e64bdb5d668)

http://securefest.canadacentral.cloudapp.azure.com:8000/files/4e0052190917969cb189bb662db630e6/word.txt?token=eyJ1c2VyX2lkIjo1LCJ0ZWFtX2lkIjpudWxsLCJmaWxlX2lkIjoxMn0.Z4sPLg.G3L_nkfP71ZyDYDjmmSkUzo611E

i try to use the cat command to see what is inside and i see this

![image](https://github.com/user-attachments/assets/15eebae8-3ec8-4f0d-8292-3b8e4562894d)

i can see the flag in the middle of the file tho 

cysssa-ctf{0y4-u-d0n-c4tch-m3}

so let move to the next warm up task

![image](https://github.com/user-attachments/assets/9ab81207-6123-4580-823a-56c22bfbbc03)

me just looking at this i already know that cysssa-ctf{y0u'r3-s7ill-sane} is the flag cos it been stated in the description tho

so let go to the next task under warm-up

![image](https://github.com/user-attachments/assets/188fc3c2-fa09-4de8-80b9-e9c9ec66c987)

while i went to the cysssa group i found the flag there 

Crypto

![image](https://github.com/user-attachments/assets/a7aaba97-bcbd-4cc6-8de0-ebc0f8fcba30)

i went ahead to decrypt it using cyberchef https://gchq.github.io/CyberChef

![image](https://github.com/user-attachments/assets/f4991d6c-201b-4c10-b3fd-ea951de783b2)
and that's the flag for welcome

SHIFT

![image](https://github.com/user-attachments/assets/330af8ab-529e-462a-983a-9b902321cc0a)

i use https://www.dcode.fr/chiffre-cesar to decrypt it

![image](https://github.com/user-attachments/assets/643ae4cf-9b1e-4984-8d09-77f49ae967e4)

i was able to get the flag while using that 

XOR
![image](https://github.com/user-attachments/assets/5dde1751-61cf-4432-a0af-7fd540aa4cd8)

i use this python script to get the flag 

``encrypted_hex = "59434949495b17594e5c414953574a565f654255486559525b56565f545d5f4700"
encrypted_bytes = bytes.fromhex(encrypted_hex)
for key in range(256):
    decrypted_bytes = bytes([byte ^ key for byte in encrypted_bytes])
    try:
        decrypted_message = decrypted_bytes.decode('utf-8')
        print(f"Key: {key:02x}, Decrypted message: {decrypted_message}")
    except UnicodeDecodeError:
        continue``

![image](https://github.com/user-attachments/assets/8812f06c-1ec4-4f7f-95ef-19096d5257b1)
i found the flag when i run the python script 

STEG
Blind

![image](https://github.com/user-attachments/assets/5ef8c1e2-1465-42bc-b95e-5b157fddfb38)

i use chatgpt to get the flag of this blind task

![image](https://github.com/user-attachments/assets/b74d55f8-a237-458a-98f8-550dfec5b491)

CHOP RICE 

![image](https://github.com/user-attachments/assets/899c8f57-bc78-4c33-8ebe-f986e941c853)

http://securefest.canadacentral.cloudapp.azure.com:8000/files/bc6ae0755c2df6f119098e6bfdd77712/jollof.png?token=eyJ1c2VyX2lkIjo1LCJ0ZWFtX2lkIjpudWxsLCJmaWxlX2lkIjo1fQ.Z4sW2A.mymVmp8WAishurmaIaxn0STrrW4

if you check the image you will see the flag
that's all i was able to solve on steg 

Rev

![image](https://github.com/user-attachments/assets/bae87b1e-812a-4751-8780-93a0a207b066)

http://securefest.canadacentral.cloudapp.azure.com:8000/files/e7aa34693dfc3eac6ecef204887196be/babyrev.zip?token=eyJ1c2VyX2lkIjo1LCJ0ZWFtX2lkIjpudWxsLCJmaWxlX2lkIjoxM30.Z4sXVA.4kEPeGUik9XltWTvN0ZIFIyzDn0

![image](https://github.com/user-attachments/assets/2595817e-936c-427f-bb05-512c8f866d5b)

and that's i was able to solve for rev 

#Web

![image](https://github.com/user-attachments/assets/30cc5b9c-eee0-4fcb-b069-2ccb58df1c3f)

in the description there was Mr Robotss, so what came to my mind is the flag is in robots.txt and i checked it out 

![image](https://github.com/user-attachments/assets/973c12bc-bfb7-4832-9fc2-8caeb281461a)

 yoo got the flag man 









        


