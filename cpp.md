<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF=8">
    <meta name="viewport" content="width=device-width, initial scale=1.0">
    <title>C++ notes</title>
</head>

<body>
    <h1>C++ Programming Notes</h1>
    <p>Programming= a way to talk to the computer</p>
    <div class="basic">
        <h3>Basic of C++</h3>
        <ul>
            <li>C++ in 1979 by Bjarne Strowstrup</li>
            <li>It is a fast n more controllable and high performance language</li>
            <li>c++11, c++14, c++17</li>
            <li><b>Streams:</b> Sequence of bytes corresponding to input or output</li>
            <li><b>Input Streams:</b> Directions of flow of bytes from input device (ex keyboard) to the main memory</li>
            <li><b>Output Streams:</b> Direction of flow of bytes from main memory to output device (ex Display)</li>
            <li>"<<" is called insertion operator(cout)</li>
            <li>">>" is called Extraction operator(cin)</li>
            <li>In c++ typecasting, int(b) is same as (int)b.</li>
            <li>We can use const keyword in c++ to make the variable immutable(can't change)</li>
            <li>(g++ -o pointer.exe pointer.cpp) to create our own exe file.</li>
            <li><b>#include (
                bits/stdc++.h>)</b></li>
        </ul>
    </div>
    <div class="variables">
        <h3>Variables</h3>
        <ul>
            <li>A container to hold data.</li>
            <li>Scope of a variable is the region in code where the existence of variable is valid.</li>
            <li>Local variables get precedance over global.</li>
            <li>To access global variable, we can use scope resolution(::) before it like ::c</li>
            <li>
                <b>Types</b>
                <ul>
                    <li><u>Local</u> (declared inside braces and can be accessed from there only)</li>
                    <li><u>Global</u> (declared outside the function and can be accessed from anywhere)</li>
                </ul>
            </li>
            <li>
                <b>Variable Types</b>
                <ul>
                    <li>int</li>
                    <li>char</li>
                    <li>float</li>
                    <li>double</li>
                    <li>boolean</li>
                    <li>string</li>
                </ul>
            </li>
            <li>
                <b>Rules to declare variables</b>
                <ul>
                    <li>var names can range from 1 to 255 characters</li>
                    <li>begin with letters or underscore</li>
                    <li>can contain digits in between name</li>
                    <li>case sensitive</li>
                    <li>no spaces or special characters allowed</li>
                    <li>can't use keyword as variable names</li>
                </ul>
            </li>
        </ul>
    </div>
    <div class="data-types">
        <h3>Data Types</h3>
        <ul>
            <li>defines the type of data a variable can hold.</li>
            <li>
                <b>Types</b>
                <ul>
                    <li><u>Built-in</u> (int, float, char, bool, double(decimal no. of high precision))</li>
                    <li><u>User-Defined</u> (Struct, Union, Enum)</li>
                    <li><u>Derived</u> (Array, Function, Pointers).</li>
                </ul>
            </li>
            <li>To speciy whether the a no.( say 34.4) is float or long double, we can use it like 34.4f and 34.4l</li>
            <li>
                <table>
                    <caption><u><b>Data types and their range</b></u></caption>
                    <tr>
                        <th>Data Type</th>
                        <th>Size(in bytes)</th>>
                        <th>Range</th>>
                    </tr>
                    <tr>
                        <td>short int</td>
                        <td>2</td>
                        <td>-32768 to 32767</td>
                    </tr>
                    <tr>
                        <td>unsigned short int</td>
                        <td>2</td>
                        <td>0 to 65535</td>
                    </tr>
                    <tr>
                        <td>int</td>
                        <td>4</td>
                        <td>-21474 to 21474</td>
                    </tr>
                    <tr>
                        <td>unsigned int</td>
                        <td>4</td>
                        <td>0 to 42949</td>
                    </tr>
                    <tr>
                        <td>long int</td>
                        <td>4</td>
                        <td>-21474 to 21473</td>
                    </tr>
                    <tr>
                        <td>unsigned long int</td>
                        <td>4</td>
                        <td>0 to 42949</td>
                    </tr>
                    <tr>
                        <td>long long int</td>
                        <td>8</td>
                        <td>-2^63 to (2^63-1)</td>
                    </tr>
                    <tr>
                        <td>unsigned long long int</td>
                        <td>8</td>
                        <td>0 to 18446744</td>
                    </tr>
                    <tr>
                        <td>signed char</td>
                        <td>1</td>
                        <td>-128 to 127</td>
                    </tr>
                    <tr>
                        <td>unsigned char</td>
                        <td>1</td>
                        <td>0 to 255</td>
                    </tr>
                    <tr>
                        <td>float</td>
                        <td>4</td>
                        <td></td>
                    </tr>
                    <tr>
                        <td>double</td>
                        <td>8</td>
                        <td></td>
                    </tr>
                    <tr>
                        <td>long double</td>
                        <td>12</td>
                        <td></td>
                    </tr>
                    <tr>
                        <td>wchar_t</td>
                        <td>2 or 4</td>
                        <td>1 wide character</td>
                    </tr>
                </table>
            </li>
            <li>
                
            <table>
                <caption><b><u>Diffrence between Primitive and Non Primitive data Type</b></u><caption></caption>
                <tr>
                    <th>Primitive</th>
                    <th>Non-Primitive</th>
                </tr>
                <tr>
                    <td>Stores the data of only one type</td>
                    <td>Stores the data of more than one type</td>
                </tr>
                <tr>
                    <td>Like int, float, char etc.</td>
                    <td>Like Arrays, Structure , Linked-list etc</td>
                </tr>
                <tr>
                    <td>Size depends on type of data structure.</td>
                    <td>Size of these is not fixed.</td>
                </tr>
                <tr>
                    <td>Starts with lowercase character.</td>
                    <td>Starts with uppercase character.</td>
                </tr>
                <tr>
                    <td>Primitive data structure can be used to call the methods.</td>
                    <td>Non-Primitive can not be used to call methods.</td>
                </tr>
            </table>
        </div>
            </li>
        </ul>
    </div>
    <div class="header-files">
        <h3>Header Files</h3>
        <ul>
            <li>
                <b>Types</b>
                <ul>
                    <li>System Header Files (<b>iostream</b> is a system header file which increases the functionality of our code)</li>
                    <li>User-Defined Files (#include (this.h))</li>
                </ul>
            </li>
            <li>iomanip is also a header file. It includes manipulators like endl(for next line), setw(num)(for setting width taken by a variable, tells the minimum number of character positions a var will consume)</li>
        </ul>
    </div>
    <div class="operators">
        <h3>Operators</h3>
        <ul>
            <li>
                <b>Types</b>
                <ul>
                    <li><u>Arithmetic Operator</u> (+, -, *, /, %, ++, --)</li>
                    <li><u>Assignment Operator</u> (=)</li>
                    <li><u>Comarision Operator</u> (==, !=, >, <, >=, <=,) </li>
                    <li><u>Logical Operator</u> (&&, ||, !)</li>
                </ul>
            </li>
            <li>When multiple operators are used, probem is solved by checking their <u>Operation precedance</u>. The one having high precedance is solved first. But if two operators are at same level, then we check their <u>Associativity</u>, it can be from right to left or from left to right.</li>
        </ul>
    </div>
    <div class="reference">
        <h3>Reference Variable</h3>
        <ul>
            <li>a variable that refers to the address of another variable( or another name given to a variable). For ex, if x=12 and &y=x, then y also print 12.</li>
            
        </ul>
    </div>
    <div class="Tricks">
        <h3>Tips and Tricks</h3>
        <ul>
            <li><b>for basic code of cpp, go to gear>>user snippets>>cpp>>write desired code in body>>prefix=keyword fr abbreviation</b></li>
        </ul>
    </div>
    <div class="pointers">
        <h3>Pointers</h3>
        <ul>
            <li>It is a data type which holds the address of another variable or data types. For ex, int a=3; and int* b= &a, here b is a pointer variable which holds the address of a.</li>
            <li>& => (Address of) Ampercent Operator</li>
            <li>* => (Value at) Dereference Operator</li>
            <li>Pointer to a pointer (means a pointer variable that stores the address of another pointer). For ex, int** c= &b, here c stores address of b. *c stores value at c(address of a) and **c stores value at a.</li>
            <li>A pointer can be incremented (++) or decremented (--).</li>
            <li>Two pointers can be subtracted.</li>
            <li>Any integer can be added or subtracted from a pointer.</li>
        </ul>
    </div>
    <div class="oops">
        <h2>Object Oriented Programming in C++</h2>
        <div class="why">
            <h3>Why OOPs</h3>
            <ul>
                <li>C++ mainly designed to add object-oriented features to C.</li>
                <li>As program size increases, readability, maintainibility and bug free nature of Program decreases. Since C relied on function or procedures(Procedural oriented programming), so possibility of not addressing the problem in effective manner was very high.</li>
                <li>Also, as data was almost neglected, so data security was easily compromised.(Any function can use any data.)</li>
                <li>Using classes solve this problem.</li>
            </ul>
        </div>
        <div class="difference">
            <h3>Diffrence between POPs and OOPs</h3>
            <table>
                <tr>
                    <th></th>
                    <th></th>
                </tr>
                <tr>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td></td>
                    <td>4</td>
                </tr>
            </table>
        </div>
        <div class="basic">
            <h3>Basics of OOPs</h3>
            <ul>
                <li><u>Classes:</u> Basic Template for creating objects.</li>
                <li><u>Objects:</u> Basic Run time entities.</li>
                <li><u>Abstraction:</u> Process of hiding implementation details and presenting only the necessary information to the user.</li>
                <li><u>Encapsulation:</u> Wrapping up the data and functions in a single unit.</li>
                <li><u>Inheritance:</u> Properties of one class can be inherited into others.</li>
                <li><u>Polymorphism:</u> Ability of functions or operators to take diffrent forms.</li>
                <li><u>Dynamic Binding:</u> Code which will execute is not known until the program runs.</li>
                <li><u>Message Passing:</u> Object message(information) call format.</li>
            </ul>

        </div>
        <div class="benifits">
            <h3>Benifits of OOPs</h3>
            <ul>
                <li>Better code reusability using Objects and Inheritance.</li>
                <li>Data hiding helps build secure systems.</li>
                <li>Multiple objects can coexist without any interference.</li>
                <li>Software complexity can be easily managed.</li>
            </ul>
        </div>
        <li>Classes are extension of structure(in C).</li>
        <li>
            Structure had limitations in C=>
            <ul>
                <li>Members are public, No data hiding.</li>
                <li>Functions can not be included in Structures.</li>
            </ul>
        </li>
        <li>In c++, structures are typedefed.</li>
        <li>Object can be declared along with the class declaration unlike in structures in c. For ex, class fruit{} mango, apple; </li>
        <li>Private data members can be accessed by using function of that class only by assigning values. They can not be accesses directly by using dot operator.</li>
        <li>Scopeof static variable is within the class.</li>
        <li>Lifespan is till program terminates.</li>
        <li>Static function is created to access only static objects.</li>
        <li>if data is input then no matter call by value and call by reference but it matters when data is passed. Values will not be swapped if & is not used, bcz in this case only formal parameters are changed.</li>
        <li>Enum serve the purpose of representing a group of named constants in a programming language</li>
        <li>Enum(X,Y,Z) is equivalent to const X=10,const Y=23; const Z=2;</li>
        <li><b>process.h</b>It includes functions for creating new processes, managing their execution and termination, and obtaining information about currently running processes.</li>
        <div class="friend">
            <h3>Friend Function</h3>
            <ul>
                <li>Friend function is not in the scope of class and so can not be called from the object of the class. For ex, c1.sumComplex()=> Invalid</li>
                <li>Can be invoked without help of Objects.</li>
                <li>Usually contains objects as arguements.</li>
                <li>Can be Declared in private or public section.</li>
                <li>It can not access data members directly, it needs object.member , because it is not in scope of class.</li>
            </ul>
        </div>
        <div class="difference">
            <h3>Diffrence between Friend Function and Member Funcion</h3>
            <table>
                <tr>
                    <th></th>
                    <th></th>
                </tr>
                <tr>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td></td>
                    <td></td>
                </tr>
                <tr>
                    <td></td>
                    <td>4</td>
                </tr>
            </table>
        </div>
        <div class="constructor">
            <h3>Constructors</h3>
            <ul>
                <li>Special member function with the same name as of the class.</li>
                <li>It is used to initialise the objects of its classes.</li>
                <li>It is invoked automatically when an object is created.</li>
                <li>It should be declared in public section of the class.</li>
                <li>Constructor do not require any return type unlike other member functions.(not any void)</li>
                <li>it can have default arguements</li>
                <li>We can not refer address of constructor.</li>
                <li>Constructor with default arguements means if any arguement missed then default arguement will be executed.(If set any). For ex, complex(int a, int b=9){}, In this if we pass complex(4), then 4, 9 will be taken and if we pass complex(4,4), then 4,4 will be taken.</li>
                <li>
                    <b>Types of constructor</b>
                    <ul>
                        <li><u>Default Constructor:</u>A constructor with no arguements.</li>
                        <li>
                            <u>Parameterised Constructor:</u>A constructor consisting of certain arguements. There can be two ways to call a constructor:
                            <ul>
                                <li><u>Implicit Call</u>, For ex, complex b(4,5).</li>
                                <li><u>Explicit Call</u>, For ex, d= complex(4,5).</li>
                            </ul>
                        </li>
                        <li>
                            <u>Copy Constructor:</u>A constructor that initializes an object using another object of the same class.
                            <ul>
                                <li>When no copy constructor is found, the compiler supplies its own copy constructor.</li>
                                <li>ex, complex(complex& obj)</li>
                            </ul>
                        </li>
                    </ul>
                </li>
                <li>If we don't use default constructor while Dynamic initialisation of objects(using multiple constructors with diffrent arguements), then it will show error as it doesn't know initially which constructor is to be called. As it is decided on run time.</li>
                <li>
                    <b>Initialisation list in Constructors</b>
                    <ul>
                        <li>It used for quick initialisation of object. [<i>Syntax: </i>complex(int a, int b): real(a), img(b){//Code to be written},where real and img are the objects of complex class.]</li>
                        <li>It is used when body of constructor is very complex.</li>
                    </ul>
                </li>
            </ul>
        </div>
        <div class="destructor">
            <h3>Destructors</h3>
            <ul>
                <li>Destructor never takes an arguement nor it returns value.</li>
                <li>To free up the space or memory taken by constructor.</li>
                <li>In basic programs, it may not matter, but is important in complex programs.</li>
            </ul>
        </div>
        <div class="Inheritance">
            <h2>Inheritance</h2>
            <div class="aboutInheritance">
                <ul>
                    <li>The concept of Reusablity in c++ is supported using inheritance.</li>
                    <li>The existing class is called as <u>Base/Super/Parent Class.</u></li>
                    <li>The new class which inherits the base class is called <u>Derived/Sub/Child Class</u></li>
                    <li>
                        <b>Types of Inheritance</b>
                        <ul>
                            <li><u>Single Inheritance:</u> A derived class with only one base class.</li>
                            <li>
                                <u>Multiple Inheritance:</u> A derived class with more than one base class.
                                <ul>
                                    <li>In multiple Inheritance, if two parents class has same function, then it creates <u>Ambiguity (I)</u> for derived class which one to use. To resolve this, we write that function using scope resolution with the class to which it belongs.</li>
                                    <li>If derived class also have same function as that of base class <u>Ambiguity (II)</u>, then it will override the function of base class.</li>
                                </ul>
                            </li>
                            <li><u>Hierarchical Inheritance:</u> Several derived class from a single base class.</li>
                            <li><u>Multilevel Inheritance:</u> Deriving a class from already derived class.</li>
                            <li>
                                <u>Hybrid Inheritance:</u> Combination of multiple and hierarchical inheritance OR combilnation of more than one type of Inheritance.
                                <ul>
                                    <li>In hybrid inheritance, a child has two fathers and they having one grandfather class in common. so both fathers have properties of grandfather. So, child gets two times those traits. To avoid this, we use virtual class. For ex, (class father1 : virtual public grandFather;) and (class father2 : virtual public grandFather;)</li>
                                    <li>If virtual keywordis not used in such case then it will give error.</li>
                                </ul>
                            </li>
                        </ul>
                    </li>
                    <li>Default visibility mode while inheriting a class is 'Private'</li>
                    <li>Private members are never inherited.</li>
                </ul>
            </div>
            <table>
                <tr>
                    <th></th>
                    <th>Public Deivation</th>
                    <th>Private Derivation</th>
                    <th>Protected Derivation</th>
                </tr>
                <tr>
                    <th>Public</th>
                    <td>Public</td>
                    <td>Private</td>
                    <td>Protected</td>
                </tr>
                <tr>
                    <th>Private</th>
                    <td>Not Inherited</td>
                    <td>Not Inherited</td>
                    <td>Not Inherited</td>
                </tr>
                <tr>
                    <th>Protected</th>
                    <td>Protected</td>
                    <td>Private</td>
                    <td>Protected</td>
                </tr>
            </table>
            <div class="consInDerived">
                <h3>Constructor in derived class</h3>
                <ul>
                    <li>If base class constructor has arguements, there is no need of constructor in derived class.</li>
                    <li>But if there are one or more arguement in constructor of base class, then derived class need to pass arguements to the constructor of base class.</li>
                    <li>If both base and derived class has constructor, then then base class constructor is executed first.</li>
                    <li>In <i>Multiple Inheritance</i> ,the base class constructor is executed in the order in the order it appear in class declaration. For ex, In (class A: public B, public C{}), constructor of (B)=>(C)=>(A) is invoked.</li>
                    <li>In <i>Multilevel Inheritance</i>, the base class constructor is executed in the order of inheritance.</li>
                    <li>The constructor for <i>Virtual Base Class</i> are invoked before an non virtual class. For ex, In (class A: public B, virtual public C{}), constructor of (C)=>(B)=>(A) is invoked.</li>
                    <li>If there are multiple virtual base class, they are invoked in the normal order.</li>
                    <li></li>
                </ul>
            </div>
        </div>
        <div class="newPointer">
            <h2>Pointers in C++</h2>
            <ul>
                <li>
                    <b>Syntax of declaring Pointer earlier and now:</b>
                    <ul>
                        <li>int a; int* p= &a;</li>
                        <li>int* ptr= new int(40); <i>(using new Keyword)</i></li>
                        <li>int* arr= new int[3]; <i>(array using new Keyword)</i></li>
                        <li>Also we can free memory by deleting the objet using delete operator. For ex, (delete [] arr;)</li>
                        <li><i>Declaring pointer in classes: </i>If we have class num, then (nums n1; nums *pt = &n1;) is same as (nums *pt = new nums;)</li>
                        <li><i>Array of object of shopItem class using pointer:</i> (shopItem* shopPtr= new shopItem[3];)</li>
                    </ul>
                </li>
                <li>
                    <b>'this' pointer</b>
                    <ul>
                        <li>It points to the object which called the member fn and using 'this' returns the same obj.</li>
                        <li>It can be used If we want to make the argument and class variable name same.</li>
                    </ul>
                </li>
                <li>
                    <b>Pointer in derived class(virtual function)</b>
                    <ul>
                        <li>Pointer of a base class can point to the object of derived class. But then the function called through that pointer , will point to the function of base class. You can directly access the functions and variables of base class only whose pointer is created. </li>
                        <li>But if we want base class pointer points to derived class pointer then we need to use virtual fn with the base class. After doing that, base class pointer points toward derived class fn. Like (virtual void base(){})</li>
                    </ul>
                </li>
            </ul>
        </div>
        <div class="polymorphism">
            <h2>Polymorphism</h2>
            <ul>
                <li>It means one name and multiple forms.</li>
                <li>
                    <b>Types of Polymorphism:</b>
                    <ul>
                        <li><b>Compile time polymorphism</b> (Early/Static binding) => [Function overloading, operator overloading.]</li>
                        <li><b>Run time polymorphism</b> () => [Virtual Functions] (Doesn't mean decision taken at run time, it means actual binding of function by compiler (associating object from its address) takes place at run time.)</li>
                    </ul>
                </li>
                <li>
                    <b>Virtual functions</b>
                    <ul>
                        <li>They can not be static.</li>
                        <li>They are accessed by object pointers.</li>
                        <li>A virtual function can be a friend of another class.</li>
                        <li>Virtual function in base class may not be used.</li>
                        <li>If a virtual function is defined in the base class, then there is no neccesity to redefine it in derived class. Means if there is no such fn in derived class it will itself search in base class, no need to redefine in derived class.</li>
                    </ul>
                </li>
                <li>
                    <b>Pure Virtual functions</b>
                    <ul>
                        <li><i>Syntax:</i> void function()=0;</li>
                        <li>It is a kind of 'do nothing function'.</li>
                        <li>It imposes on derived class that the required function should be there in derived class, if not availble, then it gives error. Base class's virtual function will not be used.</li>
                        <li>A class which is not used to create objects and used only to inherit its traits to other class is called an <b>Abstract Class.</b></li>
                    </ul>
                </li>
            </ul>
        </div>
    </div>
    <div class="fileIO">
        <h2>File Input and output in C++</h2>
        <ul>
            <li>
                <b>The useful classes for working with files in C++ are:</b>
                <ol>
                    <li>fstreambase</li>
                    <li>ifstream (derived from fstreambase).</li>
                    <li>ofstream (derived from fstreambase).</li>
                </ol>
            </li>
            <li>Use #include (fstream) to perform any file operation.</li>
            <li>
                <b>There are two ways to open a file:</b>
                <ol>
                    <li>Using the constructor ==>> ofstream out("abc.txt");</li>
                    <li>Using the member function open() of the class.</li>
                </ol>
            </li>
            <li></li>
        </ul>
    </div>
    <div class="template">
        <h2>Templates in c++</h2>
        <ul>
            <li>A template is a tool or a feature that can be used to create family of classes.</li>
            <li>We use templates to enhance reusability of code.</li>
            <li>Provide support for generic progamming.</li>
            <li><i>Syntax: </i> template (class dataType>). Here dataType can be int, float, char etc.</li>
            <li>Since a template is defined with a parameter that would be replaced by a spercified data type at the time of actual use of class/function, So they are sometimes called <b>Parameterised classes or functions.</b></li>
            <li>Template with multiple parameters=>template (class T1, class T2)</li>
            <li>Temlate with default arguements=> template (class T1=int, class T2= char)</class></li>
            <li>Outside the class a fn using template can be defined as=>template (class T>) void vasu(T>) :: displayV(){}</li>
            <li>Template functions are in which we can take desired dataType input by defining a template for it.</li>
            <li>When template functions are overloaded(means simpe function vs template fn), then exact match gets highest priority, otherwise template functions are called.</li>
        </ul>
    </div>
    <div class="STL">
        <h2>STL</h2>
        <ul>
            <li>Full form of STL is "Standard Template Library"</li>
            <li>It s the library of generic classes and function.</li>
            <li>STL is used to reuse well tested components and <i>save time</i></li>
            <li>
                <b>Components of STL</b>
                <ol>
                    <li>
                        <u>Containers</u>
                        <ul>
                            <li>Stores data, use template classes</li>
                            <li>
                                <u>Types of containers: </u>
                                <ol>
                                    <li><u>Sequence Containers</u> = Store in linear fashion. For ex, Vectors, List,  Dequeue</li>
                                    <li><u>Associative Containers</u> = Direct access. Designed such that provide fast access.All operation are fast except random access. For ex, Set, Multiset, map, Multimap </li>
                                    <li><u>Derived Containers</u> = may be derived from both of above, Real world modelling. Fast or slow depends. For ex, Stack, Queue, priority-queue</li>
                                </ol>
                            </li>
                        </ul>
                    </li>
                    <li><b>Algorithms</b> (Procedure to process data, like sorting , searching, use template functions)</li>
                    <li><b>Iterators</b> (Object points to an element in a container, connect algorithm with container, Handeled like pointers.)</li>
                </ol>
            </li>
            <li>
                <b>Vectors</b>
                <ul>
                    <li>Dynamic arrays with the ability to resize themselves automatically when an element is inserted or deleted, with their storage being handled automatically by the container.</li>
                    <li>Random access is fast</li>
                    <li>Insertion/Deletion is slow in middle</li>
                    <li>Insertion at the end is fast.</li>
                    <li>Include header file-> #include vector></li>
                    <li><i>Syntax: </i>vector(dataType) name; </li>
                </ul>
                <b>Lists</b>
                <ul>
                    <ul>allow non contiguous(non consecutive) memory allocation.</ul>
                    <li>Random access is slow (bcz iteration through pointers).</li>
                    <li>middle insertion is fast.</li>
                    <li>insertion is fast at end.</li>
                </ul>

            </li>

        </ul>
    </div>
    <li>Function Objects(Functors): Function wrapped in a class so that it is available as an object.</li>
    <li>To get these function objects we use #include functional</li>
    <li>To use sorting algorithm, we use #include algorithm</li>
    <li>conio.h header file used in C programming language contains functions for console input/output. Some of its most commonly used functions are clrscr, getch, getche, kbhit etc</li>

### git init -> Working Directory ---> git add -> staging area ---> git commit --> Repo --> git push --> Github

```
    git config --global user.name "" user.email ""
    git config --list
    git log (To check details about commit)
    git log --oneline
```

-   Since git has VIM as its default editor, which is not that easy to handle, so set vs code as its default code editor.
    For that, we need to use the command

    ```
        git config --global core.editor "code --wait"
    ```

    -   Example: _When you write **git commit** alone without using message , now instead of vim , it would open in vscode,and wait for ur changes then write commit message in the newly opened file and just close it your commit will be succesfull._

    -   .gitignore file to avoid some file to stay untracked , just write file name in the .gitignore files.

-   since git doesn't track empty folders so we use _.gitkeep_ inside that file to track that folder.

## Behind the Scenes Git

-   git snapshot is a point in time in history of your code. It is not an Image, its just a representation of code at specific point. It stores info about the code in key-value database.

## 3 Musketeers of git

-   Commit Object (inside git folder, it references tree object which furthur references blob object.)
-   Contains: - Tree Object - Parent Commit Object - Author - Committer - Commit Message
    _Example : **commit** 927bf32c829f877c664e512ec5737ef23bfcb5eb, **tree** f3eb325a62bb9c055fd09d55dc1401202dafff19, **parent** 241cc11fa403de46a622f970ad13cfacb4d1445c, **author** vasundhra gupta <vasundhragupta962@gmail.com> 1729966866 +0530, **committer** vasundhra gupta <vasundhragupta962@gmail.com> 1729966866 +0530, modify settings, cpp.md and .gitignore_

-   Tree Object (When changes/restore are done, then reference of the tree can be changed)
-   contains: - File Mode - File name - File hash - Parent Tree Object
    _Example : 100644 blob 1dcef2d9f2db74bf13c54f973f40239e00717423 .gitignore_

-   Blob Object (actual file/code that it need to save)

### Some commands to extract behind the scene Information.

```
    1.  git show -s --pretty=raw <commit-hash> (show commit object, commit hash from git log)
    2.  git ls-tree <tree-id>  (tree id from commit object, gone to upper folders and files, till get the blob, otherwise it would say not a tree object. (obvious) 😉)
    3.  git show <blob-id> (blob-id from tree object) **and this shows content of blob by blob-id**
    4.  git cat-file -p <commit-id> (get wtever next, like tree object or content)

    2nd and 4th doing work in similar way, just going to next,
```

Head points to the tip of current branch

```
    git branch <name> (create branch)
    git switch <name> (switch)
    git switch -c <name> (create and switch)
    git checkout <name> (switch)
    git branch -m <old> <new>
    git branch -d <name>
```

When changes are diffrent in files then, merge conflicts arises.

## diff and stash

-   a -> file A and b -> file B
-   ---- indicates the file A (---- doesn't mean deletion, it just indicatethe file.)
-   +++ indicates the file B
-   @@ indicates the line number

```
    git diff (doesn't do by self anything, gives info abiut diffrences in diff files of diff branches)
    *parameters more important*
    git diff <branch1> <branch2>
    git diff branch-name-one..branch-name-two
    git diff <commit-hash-one> <commit-hash-two>
```

### git stash

-   It is used when we want to save our changes at temoporary location.
-   conflicting branches soesn't allow to merge until you commit them , so use git stash to avoid this.
-   It is like a stack of changes that you can access later.

- git stash
- git stash list
- git stash save "name of stash"
- git stash apply (to revert back wat we saved on temporary location.)
- git stash apply "stash@{0}"
- git stash pop (apply and drop)
- git stash drop (drop)
- git stash clear (clear)
- git stash apply stash@{0} <branchname>

#### tags
- git tag <tagname> (not generally used, used by product managers at time of release mainly.)
- git tag -a <tag-name> -m "Release 1.0"

## git rebase and reflog
- rebase rewrites history.
rebase is always done on sub branch not main, and ensure u are on same branch u want to rebase.
(added in notes branch)
- It's like we commit something in new branch and then commit in main branch too afterwards, due to which main branch is ahead of new branch. Then we want the changes in new branch too, so we merge (which is an extra message???)

(now in main branch , due to this coming commit ,it is ahead....)

(This is a commit in main branch!! LATEST!!)

SO basically the issue is that merge commit doesnt do anything , it just merge the files, so to avoid this situation, we use rebase

- git reflog is used to give more precise history, commits
## GITHUB

### setting up ssh(Secure Shell Protocol) key
- instead of communication with id and password on command line, we gwenerate ssh key on our system , copy and give it to github, when request sent , github try to recognise  the signature (if same as your key sign or not)
- The SSH agent manages your SSH keys and remembers your passphrase.

- *To know how to generate ssh key visit github website...*
- *ssh-keygen -t ed25519 -C "vasundhragupta962@gmail.com"*

- git remote -v (to check connection)
- git remote add origin <link>
- origin  https://github.com/Vasundhra-Gupta/Cpp.git (fetch)
- origin  https://github.com/Vasundhra-Gupta/Cpp.git (push)
- meaning fetch and push from same remote repository
- git push <remotebranch name> <mybranchname>
- git push origin main
- git remove origin
- git remote add upstream <remote-url> || or you can use shorthand: git remote add -u <remote-url>
- setting upstream means , wtever pushed on main would be pushed to origin as well

</body>
</html>
