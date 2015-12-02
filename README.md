# Essentials

![cookie cutter](http://stephenmatlock.com/wp-content/uploads/2013/02/Cookie_Cutter_s.jpg)

## Object Orientation
Object-oriented programming is a way of a building new objects by making "factories" that standardize how the objects are made. Programmers don't have to code every car in GTA individually, every Facebook account, or every Amazon payment. What they do is create a template for objects that can then be tailored without having to recreate all of the code for each new object.

Object Orientation is a way to organize, manipulate and store data. It's so powerful that it gives companies like Facebook the ability to do that - Have them name apps (Instagram, Snapchat, Square or Strip, Spotify). It's one of the most important and pervasive concepts in computer programming and supports all sorts of applications like Instagram and Facebook, to ESPN to payment apps like Amazon payment.

Imagine if we had to create a dictionary for every new Facebook user.  
+ Create an instance of a Facebook user with a hash


```swift
dan b = {
  :name => "Dan B",
  :email => "dan@awesomesauce.com",
  :password => "watermelons",
  :friends => 10000000000
}
```
+ It would take forever to build a hash for each Facebook user.
  * Instead we can make a standardized template using and class.
+ Class Syntax:

```swift
  class User{
  }

  dan = User()
```
We can now easily create a new "instance" of Dan.  Think of it like creating a new cookie with a cookie cutter.  
+ Objects have descriptors (properties) and actions (methods)

```swift
  class User {
  
    let name: String = ""
    var email: String = ""
    var friends: Int = 0
    
    init(name: String, email: String, friends: Int){
     self.name = name
     self.email = email
     self.friends = friends
    }
    
  }
```
+ Let's create a new instance of our User class.  We need to initilize it with the tree values we specified in the `init()` method. The `init()` method is what gets called when we say `User.new`.
 
```swift
  lyel = User(name: "Lyel", email: "lyel@flatironschool.com, 2")
```

Cool.  So we initilized a new instance of the User class called lyel.  Here is how we can read or write the property values of our object.
```swift

  print(lyel.name)
  print(lyel.email)
  lyel.email = "lyel@whitehouse.gov"
  print(lyel.email)


```
*'lyel' is now and **instance** of the of the **User** class.  It should have values for all of the properties and all of the methods associated with that class.  We can also say that 'lyel' is an 'object.'  

Now let's make a method for the User class.  Let's say we wanted a User to be able to send a love letter. 

```swift
 class User {
  
    let name: String = ""
    var email: String = ""
    var friends: Int = 0
    
    init(name: String, email: String, friends: Int){
        self.name = name
      self.email = email
      self.firends = friends
    }
    
    func loveLetter(note: String) -> String{
      return(note + " Love, \(self.name))
    }
  
  }

print(lyel.loveLetter)
```

+ Everything is an object
  * The string `"hi"` is actually `String.new("hi")`
**Can you think of other classes and instances that we've been using all along?**

-> `UIViewContoller` is a class.  `ViewdidLoad` is a class method that tells a UIViewController instances what to do when...you guessed it, the View loads up on the ap!



<a href='https://learn.co/lessons/pc-ios-essentials-oo' data-visibility='hidden'>View this lesson on Learn.co</a>
