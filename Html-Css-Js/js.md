# Javascript
# 1. Biến
 - Quy tắc đặt tên: dùng camelCase
 - Note cần chú ý:
Array is Non-primitive.
Non-primitive data types differ from primitive data types in that they can hold more complex data. Primitive data types like strings and numbers can only hold one value at a time.
# 2. Array
 - `push`: thêm phần tử vào cuối array
 - `pop`: bỏ phần tử ở cuối array
 - `unshift`: thêm phần tử vào đầu array
 - `shift`: bỏ phần tử ở đầu array
 - `splice()`: được sử dụng để thêm, xóa hoặc thay thế các phần tử trong mảng. Hàm này sẽ thay đổi mảng gốc.

Các ví dụ:

Xoá phần tử
```javascript
let arr = [1, 2, 3, 4, 5];
let removed = arr.splice(2, 2); // Xóa 2 phần tử từ vị trí 2
console.log(arr);       // [1, 2, 5]
console.log(removed);   // [3, 4]
```
Thêm phần tử
```javascript
let arr = [1, 2, 3];
arr.splice(1, 0, 'a', 'b'); // Thêm 'a', 'b' tại vị trí 1
console.log(arr); // [1, 'a', 'b', 2, 3]
```
Thay thế phần tử
```javascript
let arr = [1, 2, 3, 4];
arr.splice(1, 2, 'x', 'y'); // Thay thế 2 phần tử tại vị trí 1 bằng 'x', 'y'
console.log(arr); // [1, 'x', 'y', 4]
```
Xoá đến hết mảng
```javascript
let arr = [1, 2, 3, 4, 5];
let removed = arr.splice(2); // Xóa tất cả phần tử từ vị trí 2
console.log(arr);       // [1, 2]
console.log(removed);   // [3, 4, 5]
```

# 3. Object
  ```javascript
  const developerObj = {
    name: "Jessica Wilkins",
    isDeveloper: true
  };

  // Object destructuring
  const { name, isDeveloper } = developerObj;
  ```
# 4. Local Storage
- `setItem()`: Dùng để lưu 1 item vào local storage.
- `getItem()`: Dùng để lấy 1 item từ local storage.
- `removeItem()`: Doá 1 item cụ thể.
- `clear()`: xoá toàn bộ item.

Eg:
```javascript
localStorage.setItem("key", value); // value could be string, number, or any other data type
```
- NOTE: Data lưu trong local Storage phải ở định dạng chuỗi.
  - Dùng JSON.stringify() với setItem()

# 6. OOP

- Định nghĩa class

```javascript
class Animal {
  constructor() {
    this.age = 16;
  }
};
```
- Từ khoá `this` dùng để chỉ đến object hiện tại.
