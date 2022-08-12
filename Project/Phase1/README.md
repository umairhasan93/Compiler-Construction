Our selected language is mini C#.
 Link to the C# language specification: https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/language-specification/introduction
Some example code for the language:


//FOR LOOP USING SINGLE DIMENSIONAL ARRAY
 using System; 
class Test { 
static void Main() { 
int[] arr = new int[5]; 
for (int i = 0; i < arr.Length; i++) 
arr[i] = i * i; 
for (int i = 0; i < arr.Length; i++) 
Console.WriteLine("arr[{0}] = {1}", i, arr[i]); 
} 
} 


// IF STATEMENT FOR AUTOMATIC MEMORY MANAGEMENT 
 using System;
 public class Stack
 {
 private Node first = null;
 public bool Empty {
 get {
 return (first == null);
 }
 }
 public object Pop() {
 if (first == null)
 throw new Exception("Can't Pop from an empty Stack.");
 else {
 object temp = first.Value;
 first = first.Next;
 return temp;
 }
 } 

//Statement lists and block statements
static void Main() {
 F();
 G();
 {
 H();
 I();
 }
} 

//switch statements
static void Main(string[] args) {
 switch (args.Length) {
 case 0:
 Console.WriteLine("No args");
 break;
 case 1:
 Console.WriteLine("One arg ");
 break;
 default:
 int n = args.Length;
 Console.WriteLine("{0} args", n);
 break;
 }
} 


//break statements
static void Main(string[] args) {
 int i = 0;
 while (true) {
 if (i == args.Length)
 break;
 Console.WriteLine(args[i++]);
 }
} 

//Classes
using System;
 class MyClass
 {
 public MyClass() {
 Console.WriteLine("Instance constructor");
 }
 public MyClass(int value) {
 MyField = value;
 Console.WriteLine("Instance constructor");
 }
 ~MyClass() {
 Console.WriteLine("Destructor");
 }
 public const int MyConst = 12;
 public int MyField = 34;
 public void MyMethod(){
 Console.WriteLine("MyClass.MyMethod");
 }
 public int MyProperty {
 get {
 return MyField;
 } 
