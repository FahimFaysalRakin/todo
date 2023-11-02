# todo

```javascript
class ToDolist {
    constructor() {
      this.order = [];
      this.delivery = [];
    }
  
    create(text) {
      this.order.push(text);
    }
  
    complete(index) {
      this.delivery.push(this.order[index]);
      this.order.splice(index, 1);
    }
  }

const todo = new ToDolist();


// orderlist
todo.create("Headphone");
todo.create("Phone Case");
todo.create("Charger");
todo.create("Wireless Chaeger");


todo.complete(1);

console.log("Order: ", todo.order);
console.log("Delivery: ", todo.delivery);
```
