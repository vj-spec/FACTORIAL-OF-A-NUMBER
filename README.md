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
```
ORG 0000H   

MOV A,#04H  

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
```
**Output:**  

<img width="1915" height="1142" alt="image" src="https://github.com/user-attachments/assets/e58aad55-002a-416c-8f1d-e2d0702ab796" />


**Manual Calculations:**  

![WhatsApp Image 2025-10-24 at 07 05 26_3b9d56b8](https://github.com/user-attachments/assets/b2e040cb-91bb-40ce-bc11-f6200952ab32)


**Result:**

Thus the factorial of a number using 8051 keil was calculated and shown the output.
