levle1

修改函数：

```
// 修改后的函数
<script>
           // 修改后的函数
        class Counter{
        constructor(){
            this.count=0;
        }
        next(){
        return this.count++;
        }
        }
        const counter=new Counter();
        for(var i=0;i<10;i++){
        console.log(counter.next())
        }

    </script>
```

结果：

<img src="C:\Users\张申树\Pictures\联想截图\联想截图_20230507225757.png" alt="联想截图_20230507225757" style="zoom: 50%;" />

创建person类：

```
class Person{
	constructor(name,age){
		this.name=name;
		this.age=age;
	}
	speak(){
		console.log('I am ${this.name},and I'm ${this.age} years old.');
	}
}
class Student extends Person{
	constructor(...courses){
		super(name,age);
		this.courses=courses;
	}
	speak() {
    	super.speak();
    	console.log(`I'm studying ${this.courses.join(', ')}.`);
  }
}
const person = new Person('CQU', 18);
person.speak();

const student = new Student('PT', 18, ['Hghtree', 'English', 'Chinses']);
student.speak(); 
```

