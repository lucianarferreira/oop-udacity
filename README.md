
# Function versus method #

A function and a method look very similar. They both use the `def` keyword. They also have inputs and return outputs. The difference is that a method is inside of a class whereas a function is outside of a class.

# **What is `self`?**

If you instantiate two objects, how does Python differentiate between these two objects?

```python
shirt_one = Shirt('red', 'S', 'short-sleeve', 15)
shirt_two = Shirt('yellow', 'M', 'long-sleeve', 20)

```

That's where `self` comes into play. If you call the `change_price` method on `shirt_one`, how does Python know to change the price of `shirt_one` and not of `shirt_two`?

```python
shirt_one.change_price(12)

```

Behind the scenes, Python is calling the `change_price` method:

```python
defchange_price(self, new_price):

        self.price = new_price

```

`Self` tells Python where to look in the computer's memory for the `shirt_one` object. Then, Python changes the price of the `shirt_one` object. When you call the `change_price` method, `shirt_one.change_price(12)`, `self` is implicitly passed in.

The word `self` is just a convention. You could actually use any other name as long as you are consisten, but you should use `self` to avoid confusing people.

![image](https://user-images.githubusercontent.com/7238176/126899651-e3992616-d376-4f65-b99b-ae567615d5de.png)

Syntax to create a new shirt object. The yntax order matches the init method. **This is called instantiating an object**.
Syntax and order match the init method. I am initializing this specific shirt with the attributes. Python is going to call the init method to initialize this shirt object.

Initializing the t-shirt:running the function, we have an output object. The output is a shirt object, and all the letters and numbers is python giving the location and memory where the object is stored. But this isn't very useful unless we store the object in a variable. So in the next slide, we will store the object in a variable. Shirt object will stored in the variable new shirt. The new shirt variable has a color, size, style and price associated with it. You can access these attributes using the dot syntax. 

Scrolling down, you use the same dot syntax to access the methods as well, except, you also need to specify any inputs that these methods require. For example, to change the price, I call the change_price method with a value of 10. Running this code you can see that the price changed from 15 to 10. The same goes for the discount method.  

![image](https://user-images.githubusercontent.com/7238176/126899809-3a420f50-87be-4079-95c6-12f6097c4a5d.png)

In the last part, I instantiate three shirt objects, and stored those objects in a list. These variables are like any other python variable.  Once he stored the shirts into the tshirt_collection list, he then ran a for loop to print out the color of each shirt. 

![image](https://user-images.githubusercontent.com/7238176/126899834-738894a8-c6cc-4bde-969a-a629db84a168.png)

![image](https://user-images.githubusercontent.com/7238176/126900579-435e1bc6-b7cf-445c-833a-e561fe465c40.png)

![image](https://user-images.githubusercontent.com/7238176/126900650-8aae74ef-df58-4767-b7db-c2e5d0afb2d6.png)





