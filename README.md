# Learn-Javascript
JavaScript là ngôn ngữ thông dịch.
ES6, ES7
Front end: Thư viện / framework JavaScript: React, Angular, Vue,...
Back end: NodeJS
Applicant: React Native
Sử dụng JavaScript để làm ngôn ngữ truy vấn : MongoDB
JavaScript engine : V8 brouser Chrome, JavaScriptCore, Nitro and SquirrelFish: trên trình duyệt Safari
API khác tên miền : CORS
Trong tab Console của Dev Tool, viết nhiều dòng Shift + Enter
Hàm: 
- Console.log() là một hàm in ra bất kể thứ gì ở console
- alert() là một hàm in ra bất kể thứ gì hiển thị dạng dialog (OK)
- confirm() thông báo trực tiếp đến người dùng ( OK và Cancel )
- prompt(title, [defaultValue]) in ra thông báo title cho phép người dùng nhập string.
- Symbol() là kiểu dữ liệu để tạo ra các unique value và bất biến 
- typeof xác định kiểu dữ tạo ra các giá trị duy nhất (unique value) và bất biến immutable.

"use strict" : đặt ở đầu gì thì toàn bộ code ở đó phải tuân theo quy tắt hiện đại
khai báo biến: let ( use strict thì phải let để định nghĩa bằng let trước khi sài )
khai báo hằng: const, khác với biến có thể thay đổi giá trị, hằng phải gán giá trị ngay sau khi khai báo

--Object
kiểu dữ liệu tham chiếu: object gồm key và value, số lượng key ( thường  Symbol() ) có thể thay đổi, giá trị ứng với key cũng có thể thay đổi
let myObject {
  key1: value1,
  key2: value2,
  key3: value3,
  ...}
Gọi thuộc tính trong object, 2 cách
- myObject[key1] bắt buộc dùng khi key chứa dấu cách, hoặc các ký tự đặc biệt khác, giá trị của key là biến hoặc biểu thức.
- myObject.key1 chỉ dùng được trong trường hợp tên thuộc tính không có kí tự đặc biệt (ngoại trừ kí tự _ và $).
kiểm tra key1 in myObject; // true
duyệt trong object: for (let prop in myObject) {} ( khai báo biến prop sẽ được gán là key1, key2, key3 và chạy hết thuộc tính trong object )
khi duyệt thì nếu là key số nguyên ( không phải số âm ) duyệt trước, nếu là key string thì theo thứ tự
arguments được thêm vào bên trong phạm vi của function, arguments chứa mảng các tham số truyền vào 

undefined chưa được gán
Riêng với dấu ` ` , có thể sử dụng biến, hằng hoặc  một biểu thức trong đó, với cú pháp ${…}.
Chuyển kiểu dữ liệu : String(), Number(), Boolean(),...
Modal window
a ?? b; tương đương a !== null && a !== undefined ? a : b;
khai báo 1 biến ngoài hàm thì có thể gán để thay đổi giá trị, nếu khai báo biến bằng let trùng tên ngoài hàm, biến ngoài hàm không dính dáng j

--Function
const bla = () {}; có nghĩa khởi tạo hàm function() và gán giá trị nó bằng 1 hằng bla, này sử cú pháp es6 tạo ra một function anonymous.
còn const bla = function() {}; là function expression, function anonymous là function expression.
Khởi tạo function có tên? nó được gọi là function declaration.
sử dụng function declartion khi muốn tạo ra function để sử dụng ở bất cứ đâu trong block ( block if else, block toàn bộ code,..)
sử dụng function expression khi function bị giới hạn vùng sử dụng, chỉ sử dụng sau khi khai , giúp global scope nhẹ và sạch hơn.
const bla = function() { return somethings }; tương đương const bla = () => somethings; , này được gọi là arrow function.
trường hợp có dấu {}, const bla = () => { return }; bạn cần sử dụng thêm từ khóa return để trả về giá trị của hàm.
truyền hàm vào hàm khác -> được gọi là callback.
Hiển thị dòng undefined khi function không return cái j
