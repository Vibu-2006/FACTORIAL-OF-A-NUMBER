# FACTORIAL-OF-A-NUMBER-USING-8051-KEIL

**AIM:**

To write and execute Assembly language Program to perform factorial of a number using 8051 keil.
APPARATUS REQUIRED: Personal computer with Keil software

**ALGORITHM:**

• Start  

• Input: Read the number n.  

• Initialize:  

•Set factorial to 1.  

•Set i to 1.  

• Loop: While i is less than or equal to n:  

•Multiply factorial by i.  

•Increment i by 1.  

• Output: Store or print the value of factorial.  

• End

**FLOW CHART:**
<img width="261" height="308" alt="image" src="https://github.com/user-attachments/assets/bffe89f6-3ba9-4294-b817-8b545f680e66" />

**Program:**

ORG 0000H   

MOV A,#06H  

MOV R0,A  

ACALL FACTORIAL  

MOV 40H,A  

SJMP THIN  

FACTORIAL:DEC R0  

CJNE R0,#01H,PRODUCT  

SJMP THICK   

PRODUCT:MOV B,R0  

MUL AB  

ACALL FACTORIAL  

THICK: RET  

THIN:  

END

**Output:**  

<img width="599" height="509" alt="Screenshot 2025-10-27 102304" src="https://github.com/user-attachments/assets/a6727e53-c531-42be-a6bf-3d0aee60cf58" />



**Manual Calculations:**  

![WhatsApp Image 2025-11-02 at 14 35 21_1b71d6d8](https://github.com/user-attachments/assets/7a609f35-bdf2-4d59-a25a-faea6bdae6b2)






**Result:**

Thus the factorial of a number using 8051 keil was calculated and shown the output.
