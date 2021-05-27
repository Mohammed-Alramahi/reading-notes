 # FUNCTIONAL PROGRAMMING

 **What is functional programming?**

 Functional programming is a programming paradigm — a style of building the structure and elements of computer programs 

 
 **What is a pure function and how do we know if something is a pure function?**

 It returns the same result if given the same arguments (it is also referred as deterministic)

 **What are the benefits of a pure function?**

  The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts

 **What is immutability?**

 When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t.

 **What is Referential transparency?**

 if a function consistently yields the same result for the same input, it is referentially transparent.

 ***

 ## Modules

 **What is a module?**

 A Javascript file.

 **What does the word ‘require’ do?**

 It will make the module that we required available to use.

 **How do we bring another module into the file that we are working in?**

 By using `require`.

 **What do we have to do to make a module available?**

 We have to export the module.
