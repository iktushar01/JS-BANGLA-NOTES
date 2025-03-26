## **🔢 Advanced Mathematical Operation Shorthand in JavaScript**

Mathematical operations (গাণিতিক অপারেশন) সহজ এবং দ্রুত করার জন্য JavaScript-এ **shorthand techniques** ব্যবহার করা হয়। শিখতে গেলে এগুলোকে **Compound Assignment Operators, Bitwise Operations, Logical Shorthands, এবং Advanced Math Methods** হিসেবে ভাগ করা যায়।

---

## **📌 1️⃣ Compound Assignment Operators (সংক্ষিপ্ত গণিত অপারেটর)**

এগুলো ব্যবহার করে গণনার **সংক্ষিপ্ত রূপে** লেখা যায়।

| **Operator** | **Shorthand** | **Equivalent To** |
| --- | --- | --- |
| `+=` | `a += b` | `a = a + b` |
| `-=` | `a -= b` | `a = a - b` |
| `*=` | `a *= b` | `a = a * b` |
| `/=` | `a /= b` | `a = a / b` |
| `%=` | `a %= b` | `a = a % b` |
| `**=` | `a **= b` | `a = a ** b` |

🔹 **উদাহরণ:**

```jsx
let a = 10;
a += 5;  // a = a + 5
console.log(a);  // Output: 15
```

---

## **📌 2️⃣ Unary Arithmetic Operators (একক অপারেটর)**

Unary অপারেটর শুধুমাত্র একটি ভেরিয়েবলের উপর কাজ করে।

| **Operator** | **Example** | **Equivalent To** |
| --- | --- | --- |
| `++` | `a++` | `a = a + 1` |
| `--` | `a--` | `a = a - 1` |
| `+` | `+a` | `Convert to Number` |
| `-` | `-a` | `Negate Value` |

🔹 **উদাহরণ:**

```jsx
let b = 5;
console.log(+b);  // Output: 5 (Number conversion)
console.log(-b);  // Output: -5 (Negative)
```

---

## **📌 3️⃣ Logical Shorthand (যুক্তিসংগত সংক্ষিপ্ত রূপ)**

**Truthy/Falsy values** এর জন্য **Logical Assignment Operators** ব্যবহার করা যায়।

| **Operator** | **Shorthand** | **Equivalent To** |
| --- | --- | --- |
| ` |  | =` |
| `&&=` | `a &&= b` | `a = a && b` |
| `??=` | `a ??= b` | `a = a ?? b` |

🔹 **উদাহরণ:**

```jsx
let x;
x ||= 10;
console.log(x);  // Output: 10 (যদি x falsy হয়, তাহলে 10 সেট হবে)

let y = 5;
y &&= 10;
console.log(y);  // Output: 10 (যদি y truthy হয়, তাহলে 10 সেট হবে)

let z = null;
z ??= 100;
console.log(z);  // Output: 100 (যদি z null/undefined হয়, তাহলে 100 সেট হবে)
```

---

## **📌 4️⃣ Bitwise Operations (বিটওয়াইজ অপারেশন)**

Bitwise অপারেশন সংখ্যা নিয়ে **বিট-লেভেল গণনা** করে।

| **Operator** | **Description** | **Example** |
| --- | --- | --- |
| `&` | AND | `5 & 3 → 1` |
| ` | ` | OR |
| `^` | XOR | `5 ^ 3 → 6` |
| `~` | NOT | `~5 → -6` |
| `<<` | Left Shift | `5 << 1 → 10` |
| `>>` | Right Shift | `5 >> 1 → 2` |
| `>>>` | Zero-fill Right Shift | `5 >>> 1 → 2` |

🔹 **উদাহরণ:**

```jsx
console.log(5 & 3);   // Output: 1 (0101 & 0011 = 0001)
console.log(5 | 3);   // Output: 7 (0101 | 0011 = 0111)
console.log(5 ^ 3);   // Output: 6 (0101 ^ 0011 = 0110)
console.log(~5);      // Output: -6 (Bitwise NOT)
console.log(5 << 1);  // Output: 10 (Left shift)
console.log(5 >> 1);  // Output: 2 (Right shift)
```

---

## **📌 5️⃣ Advanced Math Methods (উন্নত গাণিতিক পদ্ধতি)**

JavaScript-এর `Math` অবজেক্ট ব্যবহার করে গণনাগুলোকে আরও সংক্ষিপ্ত করা যায়।

| **Method** | **Example** | **Output** |
| --- | --- | --- |
| `Math.abs()` | `Math.abs(-10)` | `10` |
| `Math.floor()` | `Math.floor(4.9)` | `4` |
| `Math.ceil()` | `Math.ceil(4.1)` | `5` |
| `Math.round()` | `Math.round(4.5)` | `5` |
| `Math.sqrt()` | `Math.sqrt(25)` | `5` |
| `Math.pow()` | `Math.pow(2, 3)` | `8` |
| `Math.max()` | `Math.max(10, 5, 20)` | `20` |
| `Math.min()` | `Math.min(10, 5, 20)` | `5` |
| `Math.random()` | `Math.random()` | `0-1 এর মধ্যে যেকোনো সংখ্যা` |

🔹 **র্যান্ডম সংখ্যা তৈরি করা (১-১০ এর মধ্যে)**

```jsx
let randomNum = Math.floor(Math.random() * 10) + 1;
console.log(randomNum); // 1 থেকে 10 এর মধ্যে একটি সংখ্যা
```

---

## **📌 6️⃣ Destructuring Assignment for Math Operations**

Destructuring ব্যবহার করে গণনাগুলো সংক্ষিপ্ত করা যায়।

🔹 **একাধিক গণনা এক লাইনে**

```jsx
let [a, b] = [10, 5];
[a, b] = [a + b, a - b];
console.log(a, b);  // Output: 15, 5
```

🔹 **Array থেকে ম্যাথ অপারেশন**

```jsx
let numbers = [10, 20, 30, 40];
let sum = numbers.reduce((acc, num) => acc + num, 0);
console.log(sum);  // Output: 100
```

---

## **📌 7️⃣ Exponential Notation (বড় সংখ্যা সংক্ষিপ্ত করা)**

JavaScript বড় সংখ্যাগুলো **exponential (e) notation** ব্যবহার করে সংক্ষিপ্ত করতে পারে।

🔹 **Exponential সংখ্যা লিখা**

```jsx
let bigNumber = 5e6;  // 5000000
console.log(bigNumber);
```

🔹 **সংখ্যাকে Exponential নোটেশনে রূপান্তর করা**

```jsx
let num = 123456789;
console.log(num.toExponential(2));  // Output: 1.23e+8
```

---

## **🎯 সারসংক্ষেপ (Summary)**

✔ **Compound Assignment Operators** দ্রুত গণনার জন্য ব্যবহৃত হয়।

✔ **Unary Operators** (+, -) ব্যবহার করে দ্রুত সংখ্যা রূপান্তর করা যায়।

✔ **Logical Assignment (`||=`, `&&=`, `??=`)** মাধ্যমে ডাটা চেক করা সহজ হয়।

✔ **Bitwise Operators** উন্নত লেভেলের গণনার জন্য ব্যবহৃত হয়।

✔ **Math Object** গণনাগুলো সহজ ও সংক্ষিপ্ত করে।

✔ **Destructuring Assignment** গণনাকে আরও সহজ করে তোলে।

এখন এগুলো ব্যবহার করে নিজের কোড অপটিমাইজ করুন! 🚀
