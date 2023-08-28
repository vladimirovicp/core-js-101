## instanceof

Оператор instanceof проверяет, принадлежит ли объект к определённому классу. Другими словами, object instanceof constructor проверяет, присутствует ли объект constructor.prototype в цепочке прототипов object.

```
function Car(make, model, year) {
  this.make = make;
  this.model = model;
  this.year = year;
}
const auto = new Car('Honda', 'Accord', 1998);

console.log(auto instanceof Car);
// Expected output: true

console.log(auto instanceof Object);
// Expected output: true
```
