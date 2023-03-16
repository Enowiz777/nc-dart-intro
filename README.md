# Dart

- Dart is an OOP (Object-Oriented Programming) language that is optimized in creating UI.
- When you skip the basic and go to Flutter, you will face some difficulties.
- Nico recommends going over Dart before you move on to Flutter.
- Dart, Kotlin, Swift, and TypeScript share many similarities.

# 1 Why Dart

- Dart is optimized for UI.
- Fast on all platforms
- Dart has two souce of compilers, Dart Native and Dart Web.
- Dart Web: translate Dart to JavaScript
- Dart Native: Write Dart code and can be translated multiple architectures.
- Can be compiled JIT (Just in time) or AOT (Ahead of Time).
    - AOT: compile first and distribute resulting binary.
    - However, this is not efficient in a development. If you want to change the UI, you have to compile the whole thing again.
    - JIT resolves this issue. Uses the Dart VM to show you the result immediately. Your code runs slower because this is VM. 
    - When you are done developing, you can switch to AOT that makes the actual machine code. 
    - In conclusion, it makes the development experience easy.
- Another one is *null safety*
- Many problems that are null safe. If the develop refers to a null value, it will crash. If you have null safety, it will not crash.
- Dart and Flutter is powered by Google. 
- Therefore, you can modify the programming language to vend the rule if you want to.

# 2. How to Learn

- You can just use Dartpad as a playground to learn how to code Dart.


# 3. Hellow World

- Always have the main method to avoid error.

# 4. The Var Keyword

- You can create a variable with var.
- You specify the variable type. You can modify what is in the variable later if you want to 
- You MUST put the semi-colon to avoid an error message.
```dart
void main() {
    String name = 'Enoch';
    name = 'nico';
}
```

# 5. Dynamic Type

- Dynamic type is used when you don't know what data type you are getting inside the variable. 
- Once you get the data, Dart will help you identify which file type it is. 

# 6. Nullable Variable

- Null will cause critical error in the app. 
- There are ways to check whether the variable is null or not.
- In Dart, if you add a question makr after the Variable type, it makes it a nullable variable, which helps to eliminate the error that may be caused by a null value.

# 7. Final Variable

- If you declare you variable with Final keyword, you are not going to be able to change it later because you made it final. (version?)

# 8. Late Variable

- You will not declare the variable but when the data comes or fetches from API, you will assign data into a variable.

# 9. Constant Variable

- Values that you know that it will remain the same throughout the developmenet. 
- Need to be declared before it is sent to the app store.

# 2.0 Basic Data Type

```dart
void main() {
    String name = "nico";
    bool alive = true;
    int age = 12;
    double money = 69.99;
    // num is number that can be integer or double.
    num x = 12;
    x = 1.1;

}
// all of them are class. 

```

- String, Boolean (true or false)
- Double

# 2.1 List

- List: 
*How to create a list?*
```dart
void main() {
    List<int> numbers = [1,2,3,4];
    numbers.add(1);
    numbers.first;
    numbers.last;
}

// everything has a class or everything inherit from the object.
```
- When you make a list, try to finish with semi colon and it will change the list into a multi-line format. 
- Collection if allows you to create a list with element that may or may not be ther. 
```dart
var giveMeFive = true;
var numbers = [
    1,
    2,
    3,
    4,
    if (giveMeFive) 5,
    // if giveMeFive is true add 5 to the list.
]
```

## 2.2 String interpolation


```dart
void main() {
    var name = 'nico';
    var age = 10;
    var greeting = 'Hello everyone, my nem is $name
    and I'm ${age + 2}';

    print(greeting);

}
```
- rules: choose double quote if you want.
- If you use the money sign($), you have to include a variable. 
- You can include the operation inside the curly bracket{};
- 