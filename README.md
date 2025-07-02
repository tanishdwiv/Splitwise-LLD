# 💸 Splitwise - Low Level Design (LLD) Project

This is a low-level design (LLD) implementation of the popular expense-splitting application **Splitwise**, written in Java. The project allows users to form groups, add expenses, split bills using various strategies (Equal, Unequal, and Percentage), and view/update balances between users.

---

## 🚀 Features

- 👥 User and Group management
- ➗ Expense splitting using:
  - Equal Split
  - Unequal Split
  - Percentage Split
- 📊 Real-time balance tracking
- 🧮 Modular design following object-oriented principles

---

## 📂 Project Structure

```
splitwiselld/
├── src/
│   └── main/
│       └── java/
│           └── org/example/
│               ├── Balance/
│               ├── Controllers/
│               ├── Expense/
│               ├── Group/
│               ├── Split/
│               ├── User/
│               ├── Main.java
│               └── Splitwise.java
├── pom.xml
└── README.md
```

---

## ⚙️ Getting Started

### 🛠 Prerequisites

- Java JDK 8 or above
- Git (for cloning)
- Maven (optional, but recommended)
- Any IDE (IntelliJ, Eclipse, VS Code)

### 📥 Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/splitwiselld.git
cd splitwiselld
```

### 🧱 Step 2: Compile and Run

#### With Maven:

```bash
mvn clean compile
mvn exec:java -Dexec.mainClass="org.example.Main"
```

#### Without Maven (Manual):

```bash
javac -d out src/main/java/org/example/**/*.java
java -cp out org.example.Main
```

---

## 🧪 Sample Output

```
Tanish owes Rahul: 500.0
```

This is based on a sample expense where Tanish paid ₹1000 split equally with Rahul.

---

## 📌 Core Classes

| Class | Responsibility |
|-------|----------------|
| `User` | Represents a system user |
| `Group` | Manages a group of users |
| `Expense` | Represents a transaction |
| `Split` | Abstract base for different splitting logic |
| `EqualExpenseSplit`, `UnequalExpenseSplit`, `PercentageExpenseSplit` | Implements respective logic |
| `UserExpenseBalanceSheet` | Tracks balances for each user |
| `Splitwise` | Main class that ties everything together |

---

## 📜 License

This project is released under the **MIT License** and is intended for educational and demo purposes.

---

## 👤 Author

**Tanish Dwivedi**  
[GitHub](https://github.com/your-username)

---

> Inspired by the core idea behind Splitwise to demonstrate object-oriented design in Java.
