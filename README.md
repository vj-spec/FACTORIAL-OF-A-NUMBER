# FACTORIAL-OF-A-NUMBER-USING-8051-KEIL

**AIM:**

To write and execute Assembly language Program to perform factorial of a number using 8051 keil.
**APPARATUS REQUIRED:** Personal computer with Keil software

**Algorithm**

1. **Start**
2. **Input:** Read the number `n`.
3. **Initialize:**
   * Set `factorial = 1`
   * Set `i = 1`
4. **Loop:** While `i` ≤ `n`
   * Multiply `factorial` by `i`
   * Increment `i` by 1
5. **Output:** Store or print the value of `factorial`.
6. **End**

   
**FLOW CHART:**

<img width="261" height="200" alt="image" src="https://github.com/user-attachments/assets/bffe89f6-3ba9-4294-b817-8b545f680e66" />

**Program:**
```
ORG 0000H
	MOV DPTR, #4500H
	MOVX A,@DPTR
	MOV R0,A
	INC DPTR
	ACALL FACTORIAL
	MOVX @DPTR,A
	SJMP THIN 
	FACTORIAL: DEC R0
	CJNE R0,#01H,PRODUCT
	SJMP THICK
	PRODUCT:MOV B,R0
	MUL AB
	ACALL FACTORIAL
	THICK: RET
	THIN: RET
	END
```
**Output:**  

<img width="500" height="420" alt="image" src="https://github.com/user-attachments/assets/e58aad55-002a-416c-8f1d-e2d0702ab796" />


**Manual Calculations:**  

<img width="500" height="420" alt="image" src="https://github.com/user-attachments/assets/b2e040cb-91bb-40ce-bc11-f6200952ab32" />


**Result:**

Thus the factorial of a number using 8051 keil was calculated and shown the output.
