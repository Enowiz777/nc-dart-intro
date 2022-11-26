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