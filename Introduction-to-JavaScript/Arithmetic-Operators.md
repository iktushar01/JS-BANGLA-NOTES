## **🔢 Introduction to Arithmetic Operators in JavaScript**

Arithmetic operators (গাণিতিক অপারেটর) হলো JavaScript-এর একটি গুরুত্বপূর্ণ অংশ, যা গাণিতিক গণনার জন্য ব্যবহৃত হয়। এগুলো সংখ্যা নিয়ে কাজ করে এবং ফলাফল হিসেবে একটি সংখ্যা প্রদান করে।

---

### **📌 1️⃣ Arithmetic Operators List**

| **Operator** | **Name (নাম)** | **Example (উদাহরণ)** | **Result (ফলাফল)** |
| --- | --- | --- | --- |
| `+` | Addition (যোগ) | `5 + 3` | `8` |
| `-` | Subtraction (বিয়োগ) | `10 - 4` | `6` |
| `*` | Multiplication (গুণ) | `6 * 3` | `18` |
| `/` | Division (ভাগ) | `12 / 4` | `3` |
| `%` | Modulus (ভাগশেষ) | `10 % 3` | `1` |
| `**` | Exponentiation (ঘাত/পাওয়ার) | `2 ** 3` | `8` |

---

## **📌 2️⃣ Explanation of Arithmetic Operators (বিস্তারিত ব্যাখ্যা)**

### **1. Addition (`+`) - যোগ করা**

এই অপারেটর দুটি সংখ্যাকে যোগ করতে ব্যবহার করা হয়।

```jsx
let sum = 5 + 3;
console.log(sum);  // Output: 8
```

📌 **বিশেষ দ্রষ্টব্য:** যদি স্ট্রিং (`"5" + "3"`) থাকে, তাহলে এটি সংখ্যা যোগ না করে স্ট্রিং সংযোজন (concatenation) করবে।

```jsx
console.log("5" + "3");  // Output: "53"
```

---

### **2. Subtraction () - বিয়োগ করা**

এই অপারেটর দুটি সংখ্যার মধ্যে বিয়োগফল নির্ধারণ করে।

```jsx
let difference = 10 - 4;
console.log(difference);  // Output: 6
```

---

### **3. Multiplication () - গুণ করা**

এই অপারেটর দুটি সংখ্যাকে গুণ করতে ব্যবহৃত হয়।

```jsx
let product = 6 * 3;
console.log(product);  // Output: 18
```

---

### **4. Division (`/`) - ভাগ করা**

এই অপারেটর প্রথম সংখ্যাকে দ্বিতীয় সংখ্যার দ্বারা ভাগ করে।

```jsx
let quotient = 12 / 4;
console.log(quotient);  // Output: 3
```

📌 **শূন্য দ্বারা ভাগ করলে Infinity বা NaN পাওয়া যায়:**

```jsx
console.log(10 / 0);  // Output: Infinity
console.log(0 / 0);   // Output: NaN (Not a Number)
```

---

### **5. Modulus (`%`) - ভাগশেষ নির্ণয় করা**

এই অপারেটর প্রথম সংখ্যাকে দ্বিতীয় সংখ্যা দিয়ে ভাগ করে **ভাগশেষ (remainder)** প্রদান করে।

```jsx
let remainder = 10 % 3;
console.log(remainder);  // Output: 1
```

📌 **Modulus অপারেটর ব্যবহার করা হয় সংখ্যাকে জোড় (even) বা বিজোড় (odd) চেক করার জন্য:**

```jsx
let num = 7;
if (num % 2 === 0) {
  console.log("Even Number");
} else {
  console.log("Odd Number");
}
// Output: Odd Number
```

---

### **6. Exponentiation (`*`) - ঘাত বা পাওয়ার**

Exponentiation অপারেটর ব্যবহার করে একটি সংখ্যার উপর ঘাত (power) নির্ধারণ করা যায়।

```jsx
let power = 2 ** 3;  // 2^3 = 8
console.log(power);   // Output: 8
```

📌 **`Math.pow()` ব্যবহার করেও একই কাজ করা যায়:**

```jsx
console.log(Math.pow(2, 3));  // Output: 8
```

---

## **📌 3️⃣ Increment & Decrement Operators**

সংখ্যার মান ১ করে বাড়ানো বা কমানোর জন্য Increment (`++`) এবং Decrement (`--`) অপারেটর ব্যবহার করা হয়।

### **1. Increment (`++`) - সংখ্যা ১ করে বাড়ানো**

```jsx
let count = 5;
count++;
console.log(count);  // Output: 6
```

### **2. Decrement (`-`) - সংখ্যা ১ করে কমানো**

```jsx
let count2 = 5;
count2--;
console.log(count2);  // Output: 4
```

📌 **Prefix এবং Postfix Increment/Decrement পার্থক্য:**

```jsx
let x = 5;
console.log(++x);  // Output: 6 (প্রথমে বৃদ্ধি, পরে প্রদর্শন)
console.log(x++);  // Output: 6 (প্রথমে প্রদর্শন, পরে বৃদ্ধি)
console.log(x);    // Output: 7
```

---

## **📌 4️⃣ Combining Assignment with Arithmetic Operators**

সংখ্যার মান পরিবর্তনের জন্য **Compound Assignment Operators** ব্যবহার করা হয়।

| **Operator** | **Example** | **Equivalent To** |
| --- | --- | --- |
| `+=` | `a += 5` | `a = a + 5` |
| `-=` | `a -= 3` | `a = a - 3` |
| `*=` | `a *= 2` | `a = a * 2` |
| `/=` | `a /= 4` | `a = a / 4` |
| `%=` | `a %= 3` | `a = a % 3` |
| `**=` | `a **= 2` | `a = a ** 2` |

🔹 **উদাহরণ:**

```jsx
let a = 10;
a += 5;  // a = a + 5
console.log(a);  // Output: 15
```

---

## **📌 5️⃣ Math Object (গাণিতিক গণনার জন্য)**

JavaScript-এ উন্নত গণনার জন্য `Math` অবজেক্ট ব্যবহার করা হয়।

| **Math Function** | **Example** | **Output** |
| --- | --- | --- |
| **Math.round()** | `Math.round(4.7)` | `5` |
| **Math.floor()** | `Math.floor(4.9)` | `4` |
| **Math.ceil()** | `Math.ceil(4.2)` | `5` |
| **Math.random()** | `Math.random()` | `0-1` এর মধ্যে যেকোনো সংখ্যা |
| **Math.sqrt()** | `Math.sqrt(25)` | `5` |
| **Math.abs()** | `Math.abs(-10)` | `10` |

🔹 **র্যান্ডম সংখ্যা তৈরি করা:**

```jsx
let randomNum = Math.floor(Math.random() * 10) + 1;
console.log(randomNum);  // 1 থেকে 10 এর মধ্যে র্যান্ডম সংখ্যা
```

---

## **🎯 সারসংক্ষেপ (Summary)**

- **Arithmetic Operators** হল `+`, , , `/`, `%`, `*`।
- **Increment (`++`) & Decrement (`-`)** সংখ্যা বাড়ানো বা কমানোর জন্য ব্যবহৃত হয়।
- **Compound Assignment Operators** (`+=`, `=`, `=`, `/=`, `%=`) গণনা সহজ করে।
- **Math Object** উন্নত গণনার জন্য ব্যবহার করা যায়।

এখন এগুলো ব্যবহার করে নিজে কোড লিখুন এবং প্র্যাকটিস করুন! 🚀
