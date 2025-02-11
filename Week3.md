### **🔥 Hackathon Assignment: ATM System using Python 🏧**  

📌 **Objective:** Build a **basic ATM system** that allows users to perform banking operations like balance inquiry, withdrawals, deposits, and PIN authentication.  

---

### **🔹 Key Features:**  
✅ **User Authentication:** Prompt users to enter a PIN before accessing their account.  
✅ **Balance Inquiry:** Display the current account balance.  
✅ **Withdraw Money:** Allow users to withdraw money (ensure sufficient balance).  
✅ **Deposit Money:** Enable users to deposit money into their account.  
✅ **Exit Option:** Provide an option to exit the ATM system gracefully.  

---

### **🛠️ Expected Implementation Steps:**  
1️⃣ **Create a Python script (`atm.py`).**  
2️⃣ **Define a dictionary to store user PINs and balances.**  
3️⃣ **Implement a login system:** Prompt the user for a PIN and validate it.  
4️⃣ **Display a menu with options:**  
   - Check balance  
   - Deposit money  
   - Withdraw money  
   - Exit  
5️⃣ **Handle transactions properly:** Ensure the user can't withdraw more than their balance.  
6️⃣ **Loop the system** until the user chooses to exit.  

---

### **✨ Example Output Expectations:**  

```
Welcome to the ATM 🏧
Enter your PIN: ****
Login successful ✅

Choose an option:
1. Check Balance
2. Deposit Money
3. Withdraw Money
4. Exit
Enter your choice: 2
Enter deposit amount: 1000
Deposit successful! Your new balance is $2000.

Choose an option: 3
Enter withdrawal amount: 500
Withdrawal successful! Your remaining balance is $1500.

Choose an option: 4
Thank you for using our ATM. Goodbye! 👋
```

---

### **💡 Bonus Challenges:**  
🔥 **Use OOP (Object-Oriented Programming)** to structure the ATM system with classes (`ATM`, `Account`).  
🔥 **Store user data in a file (`users.json` or `users.txt`)** instead of a dictionary for persistence.  
🔥 **Implement a retry system**: Lock the account after 3 incorrect PIN attempts.  
🔥 **Add transaction history tracking** for deposits and withdrawals.  

---

This **Python mini-project** is **great for practicing functions, conditionals, loops, and user input handling!** 🚀 Let me know if you want a **starter template or additional features!** 💪🔥
