### Strings Exercises

#### S1.
Without using string interpolation, print out a string that combines myGreeting and myName.

```
let myGreeting = "Hello, "
let myName = "Ben"

print(myGreeting, myName)
```


#### S2.
Write code that prints out myArray as a single string separated by spaces.



```swift
let myArray = ["Hi", "there,", "how","is","it","going?"]

for i in 0..<myArray.count {
    print("\(myArray[i])", terminator: " ")
}

```
#### S3.
Write code that prints out all the numbers from 1 to 10 as a single string.  (Hint: the String() function can convert an int to a string)

for i in 1...10 {
print("\(i)", terminator: " ")
}

or 

var myString = [String]()

for i in 1...10{
    myString.append(String(i))
}

#### S4.
Write code that prints out all the even numbers from 5 to 51 as a single string.

for i in 5...51 {
if i%2 == 0{
print("\(i)", terminator: " ")
}
}

#### S5.
Write code that prints out every number ending in 4 between 1 and 60 as a single string.

for i in 1...60 {
if i%10 == 4{
print("\(i)", terminator: " ")
}
}

#### S6.
Print each character in the string ```var world = "Hello world!"

for i in world.characters {
print(i, terminator: " ")
}
```



#### S7.
Using '.characters' and loop, print the last character in the string below
```swift
let myStringSeven = "Hello world!"

```

#### S8.
Write code that switches on a string.  If the string's length is even, print out every character.  If the string's length is odd, print out every other character

let myString = "abcdefgh"

switch myString {
    case let _ where myString.characters.count %2 == 0:
        for i in myString.characters{
    print(i)
}
    default:
    var j = 1
for k in myString.characters {
        if j % 2 ==0 {
        print(k)
}
    }
}

#### S9.
Initialize a String with a character. Show that it is a Character, and not another String, you're using
to initialize it.



### Unicode exercises

#### U1.
Build five pairs of canonically equivalent strings, the first of each being a pre-composed character and
the second being one that uses combinable unicode scalars. Show that they are equivalent.

Refer to this [Unicode Table](http://unicode-table.com/en/).

#### U2.
* Using only Unicode, print out "HELLO WORLD!"
var first = "\u{0048}\u{0045}\u{004C}\u{004C}\u{004F}\u{0020}\u{0057}\u{4F}\u{52}\u{4C}\u{44}"
#### U3.
* Using only Unicode, print out your name.

#### U4
* (Bonus) Using only Unicode, print "Hello World" in another language.

#### U5.
Print the below flower box using the following information.
* The unicode number for ⚘ is U-2698
* The top and bottom of the box are represented by dashes and the rows are ```|```
* Use the __terminator__ argument in your print statements to print on the same line.
* Hint: It may be useful to try printing out a box of just one character to start then work your way from there.

```
- - - - - - - - - - -
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
- - - - - - - - - - -

```