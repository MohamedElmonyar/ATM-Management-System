
# 🏧 ATM Management System - C++

A simple console-based ATM system built using C++. This project simulates core ATM functionalities such as deposit, withdrawal (normal and quick), and balance inquiry, with persistent storage through a text file.

---

## 📌 Features

- 🔐 **Login system** with Account Number and PIN code  
- 💵 **Quick Withdraw** options (20, 50, 100, ..., 1000)  
- 💸 **Normal Withdraw** with custom amount (must be multiple of 5)  
- 💰 **Deposit funds** with amount validation  
- 🧾 **Check Balance**  
- 💾 **Client data saved to `Clients.txt`** for persistence  

---

## 🗃️ Data Structure

```cpp
struct sClient {
    string AccountNumber;
    string PinCode;
    string Name;
    string Phone;
    double AccountBalance;
    bool MarkForDelete = false;
};
```

---

## 🧾 Data Format

Each client's data is stored in a text file using the delimiter `#//#`.  
Example:
```
12345#//#9999#//#John Doe#//#1234567890#//#1500.75
```

---

## 🛠️ Technologies Used

- **Language:** C++  
- **I/O:** fstream  
- **Structures:** Vectors, Structs  
- **IDE:** Visual Studio 2022  
- **Platform:** Windows Console  

---

## ⚠️ Disclaimer

This is an educational project and does **not** include encryption or secure storage of sensitive information. Not intended for real-world financial use.

---

## 🧑‍💻 Author

Mohamed Elmonier

---

## ✅ How to Run

1. Open the project in **Visual Studio 2022**  
2. Make sure `Clients.txt` is in the same directory as the executable  
3. Build and run the program  
4. Login with existing account data from the file
