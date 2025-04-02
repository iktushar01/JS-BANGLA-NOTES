## **🔍 Compare Variables and Comparison Operators in JavaScript**

### **🔹 1️⃣ What is Variable Comparison?**

ভেরিয়েবল কম্পারিজন হল দুটি বা ততোধিক মান তুলনা করা এবং ফলাফল **true** অথবা **false** পাওয়া। JavaScript-এ তুলনা করতে **Comparison Operators** ব্যবহার করা হয়।

---

## **📌 2️⃣ Types of Comparison Operators (তুলনার অপারেটরসমূহ)**

### **✅ Equality Operators (সমান কি না চেক করা)**

| **Operator** | **Description** | **Example** | **Output** |
| --- | --- | --- | --- |
| `==` | Equal to (value check) | `5 == "5"` | `true` |
| `===` | Strict equal (value + type check) | `5 === "5"` | `false` |
| `!=` | Not equal (value check) | `5 != "5"` | `false` |
| `!==` | Strict not equal (value + type check) | `5 !== "5"` | `true` |

🔹 **উদাহরণ:**

```jsx
console.log(5 == "5");   // true (value same, type check করেনি)
console.log(5 === "5");  // false (value same, but type different)
console.log(10 != "10"); // false (value same, type check করেনি)
console.log(10 !== "10");// true (value same but type different)
```

---

### **✅ Relational Operators (বড়, ছোট, বড়-সমান, ছোট-সমান)**

| **Operator** | **Description** | **Example** | **Output** |
| --- | --- | --- | --- |
| `>` | Greater than (বড়) | `10 > 5` | `true` |
| `<` | Less than (ছোট) | `5 < 10` | `true` |
| `>=` | Greater than or equal (বড় বা সমান) | `10 >= 10` | `true` |
| `<=` | Less than or equal (ছোট বা সমান) | `5 <= 10` | `true` |

🔹 **উদাহরণ:**

```jsx
console.log(10 > 5);  // true
console.log(5 < 10);  // true
console.log(10 >= 10); // true
console.log(5 <= 2);  // false
```

---

### **✅ Logical Comparison (যৌক্তিক অপারেটর + তুলনা)**

| **Operator** | **Description** | **Example** | **Output** |
| --- | --- | --- | --- |
| `&&` | AND (উভয় সত্য হলে true) | `(5 > 2) && (10 > 5)` | `true` |
| ` |  | ` | OR (যেকোনো একটি সত্য হলে true) |
| `!` | NOT (ফল উল্টো করে) | `!(5 > 2)` | `false` |

🔹 **উদাহরণ:**

```jsx
console.log((10 > 5) && (20 > 15)); // true (উভয় শর্তই সত্য)
console.log((10 > 5) || (20 < 15)); // true (একটি সত্য হলে true)
console.log(!(10 > 5)); // false (NOT উল্টো করে)
```

---

## **📌 3️⃣ Difference Between `==` and `===` (Double vs Triple Equals)**

| Operator | Checks | Example | Output |
| --- | --- | --- | --- |
| `==` | Value only | `5 == "5"` | `true` |
| `===` | Value + Type | `5 === "5"` | `false` |

🔹 **উদাহরণ:**

```jsx
console.log(5 == "5");  // true (value same)
console.log(5 === "5"); // false (value same, but type different)
console.log(0 == false);  // true (0 is falsy)
console.log(0 === false); // false (type different)
```

---

## **📌 4️⃣ Comparing Strings & Numbers**

**String তুলনা ASCII value দিয়ে হয়** এবং **সংখ্যা তুলনা সরাসরি সংখ্যার উপর ভিত্তি করে হয়।**

🔹 **String comparison (অক্ষর গুলোর ASCII value অনুযায়ী চেক হয়)**

```jsx
console.log("apple" > "banana"); // false ('a' এর ASCII 97, 'b' এর ASCII 98)
console.log("hello" < "world");  // true ('h' < 'w')
console.log("Zoo" > "apple");   // false ('Z' এর ASCII 90, 'a' এর ASCII 97)
```

🔹 **String vs Number comparison**

```jsx
console.log("5" > 3);   // true ('5' → number 5, 5 > 3)
console.log("10" < 2);  // false ('10' → number 10, 10 < 2 ভুল)
console.log("100" == 100); // true ('100' → number 100)
```

---

## **📌 5️⃣ Special Cases in Comparison**

🔹 **Null এবং Undefined তুলনা:**

```jsx
console.log(null == undefined); // true (বিশেষ নিয়ম)
console.log(null === undefined); // false (type different)
console.log(null > 0);  // false (null কে 0 ধরা হয় না)
console.log(null == 0); // false (বিশেষ নিয়ম)
console.log(null >= 0); // true (বিশেষ নিয়ম)
```

🔹 **NaN (Not a Number) তুলনা:**

```jsx
console.log(NaN == NaN);  // false (NaN কখনোই NaN-এর সমান নয়)
console.log(NaN === NaN); // false (NaN is unique)
console.log(isNaN(NaN));  // true (NaN চেক করার জন্য isNaN() ব্যবহার করতে হয়)
```

---

## **🎯 সারসংক্ষেপ (Summary)**

✔ **`==` শুধু মান চেক করে, `===` মান এবং টাইপ দুটোই চেক করে।**

✔ **`!=` এবং `!==` অপারেটর ভিন্নতা চেক করে।**

✔ **`>`, `<`, `>=`, `<=` সংখ্যার তুলনা করে।**

✔ **Logical operators (`&&`, `||`, `!`) শর্ত যাচাই করতে ব্যবহৃত হয়।**

✔ **Null, Undefined এবং NaN তুলনার সময় সতর্ক হতে হবে।**
