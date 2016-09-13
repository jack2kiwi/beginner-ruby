## Ruby 101
### By: Jack Holland
#### What is Rubery???
Well, first of all, it is Ruby not Rubery. Ruby is a coding language that is used to build and create websites and is the base of the language _Rails_. To understand the basics of Ruby you must first learn about _variables_, _conditionals_, and _methods_.
#### Variables
* ##### Assigning Variables/Types of Variables
    * Assigning variables is actually very simple. Before you are able to use them you have to assign a number (integer or float), string, or condition (boolean) to the variable
        * ###### Integer/Float:
        Integers are whole numbers while floats are decimals.
        Assigning a variable as an integer is very simple, you just type the variable, put an equal sign, and then type the number like so:
        ```
        cats = 3
        ```

        Sometimes it is best to use floats instead of integers because when altering your integer it may become a decimal but cannot be written out as one.
        Assigning a variable as a float is very similar to that of an integer. You follow the same steps but just put at least a number in the tenths place at the end like this:
        ```
        lives = 7.0
        ```

        * ###### String:
        A string can be a sentence, a word, or a single letter/character.
        To assign a string to a variable you can put either single or double quotation marks around the string like so:
        ```
        cat_says = "meow"
        ```

        * ###### Boolean:
        A boolean is a true or false statement.
        To assign a boolean to a variable you can set the variable equal to simply true or false like this:
        ```
        cool_cat = true
        ```
* ##### Using Variables
    * Variables can be compared, put in strings, and many more
        * ###### Comparing variables:
        Variables can be compared in things such as if statements (these will be explained later on) to see if an action should be done like so:
        ```
        if cats * 2 == lives
            puts "Each cat has an average of 2 lives"
        end
        ```

        * ###### Returning variables in strings
        Variables can be returned in strings by placing a #{} around the variable in the string like so:
        ```
        puts "There are #{cats} cats and they have #{lives} combined"
        ```


#### Conditionals
    * Conditionals are statements that check if something is true, and if it is they end up doing something
    * ##### Expressions
        * There are two main types of expressions in ruby: if statements and while loops
        * ###### If Statements
            * If statements see if the condition that they are given is true, if so they do something.
            They can check if another condition is true if the first one isn't with an elsif.
            Also, they can also do something if none of the conditions described are true with an else.
            Using else and elsif is known as __branching__ your if statement
            They can be used like this:
            ```
            cars = 2

            if cars == 0
                puts "There are no cars"
            elsif cars.between?(1, 3)
                puts "There are some cars"
            else
                puts "There are a lot of cars"
            end
            ```
        * ###### While loops
            * While loops complete a function while a given condition is true. While loops must always be able to end other wise they will go on forever
            Here is an example of how to use one:
            ```
            gas = 20

            while gas > 0
                gas -= 1
            end
            puts "YOU RAN OUT OF GAS!"
            ```
            * This while loops will run 20 times, each time the amount of gas is decreased by one. When the gas is no longer more than 0, the while loop will no longer run and the code will say that you have ran out of gas


#### Methods
    * Methods are some sort of machine where you put some inputs in and it returns an output, just like a toaster where you put in bread and are returned toast. To use a method you must first define the method and then give the method the inputs
    * ##### Defining Methods
        * To define a method you must always use a define block to tell your code what to do with the input so it can return an output. They are written like this:
        ```
        def smaller_number(a)
            smaller_number = a - 12
            return smaller_number
        end
        ```
        * This is a very simple method that will return a number 12 smaller than the number that was inputed which in this case is called a.
    * ##### Supplying an Input
        * Supplying a method is very simple. All you have to do is use the method but put some kind of number, string, or boolean in the method based on what it requires rather than using an undefined variable like so:
        ```
        def smaller_number(a)
            smaller_number = a - 12
            return smaller_number
        end

        smaller_number(3478)
        ```
        * See, wasn't that easy. Now the method will return a number that is smaller than the number that we inputed. The number that will be returned in this case is 3466.
