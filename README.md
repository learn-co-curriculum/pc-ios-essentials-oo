# Essentials

![cookie cutter](http://stephenmatlock.com/wp-content/uploads/2013/02/Cookie_Cutter_s.jpg)

## Object Orientation
The answer is through a type of programming called object-oriented programming. It's a way a building new objects (alien enemies, Sim people, cars, etc.) by making "factories" that standardize how the objects are made. Programmers don't have to code every car in GTA individually, every Facebook account, or every Amazon payment. What they do is create a template for objects that can then be tailored without having to recreate all of the code for each new object. The same goes for applications like Facebook and Twitter.

Object Orientation is a way to organize, manipulate and store data. It's so powerful that it gives companies like Facebook the ability to do that - Have them name apps (Instagram, Snapchat, Square or Strip, Spotify). It's one of the most important and pervasive concepts in computer programming and supports all sorts of applications like Instagram and Facebook, to ESPN to payment apps like Amazon payment. In fact, you guys are going to build your own payment system tomorrow.

Who knows how many people are on Facebook? Close to a quarter of the world is on Facebook (roughly 2billion). What do you think the average number of friends a user has? What about the number of photos? How many likes happen in a day? We're talking about trillions of pieces of data that Facebook tracks and stores on huge tracks on land that they bought literally just to store all their data.

When you log in, how does Facebook know to your data? Your exact profile and data loaded for you and you alone, and not someone else's? How does that work? How in the world are they able to do that for 2 billion users?

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
  class User
  end

  dan = User.new
```
We can now easily create a new "instance" of Dan.  Think of it like creating a new cookie with a cookie cutter.  
+ Objects have descriptors (properties) and actions (methods)
+ Instance variables require one method to exist called the **reader** method:
```swift
  class User
  
    let name: String = ""
    var email: String = ""
    var friends: Int = 0
    
    Init(name: String, email: String, friends: Int){
    }
    
  end
```
+ If we want to be able to change the value of the instance variable like a user's age, a second method is required called a **writer** method:
```swift
  lyel = User.New(name: "Lyel", email: "lyel@flatironschool.com, 2)
  
  print(lyel.name)
  print(lyel.email)
  lyel.email = "lyel@whitehouse.gov"
  print(lyel.email)

  end
```

+ Everything is an object
  * The string `"hi"` is actually `String.new("hi")`
    * Shortcut is just syntactic sugar
  * Same for arrays, integers, hashes, etc.
  * We can add methods to existing classes
```ruby
  class Array
    def say_items
      puts "The items in this array are:"
      self.each do |item|
        puts item
      end
    end
  end
```





+ Get students to understand that anything can be turned into a class with attributes and actions. Pick 
+ 
+What classes have you seen already?  UIViewContoller is a class.  ViewdidLoad is a class method that tells a UIViewController instances what to do when...you guessed it, the View loads up on the ap!

+Come up with at least the properties and two methods for the following:
+ An instagram post
+ A spotify playlist
+ A song in spotify
+ A snap from snapchat
