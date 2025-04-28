# ece39595-homework-4-solved
**TO GET THIS SOLUTION VISIT:** [ECE39595 Homework 4 Solved](https://www.ankitcodinghub.com/product/ece39595-homework-4-solved-3/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;119768&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;ECE39595 Homework 4 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Homework 4 will focus on operator overloading. Some of the code is provided, and some of this code shows a couple of neat tricks we can do in C++, one involving a clever use of references and the other involving delegating constructors.

In this homework you will be developing a 2D Array class (Array2D), and you need to implement some of the functionality associated with such a class. In particular, you will implement the following functions.

Functions to implement:

Array2D(const Array2D&amp; other): A copy constructor. The storage of the initialized 2D array representing the actual array data should be different than the storage of the data of the other 2D array’s array data. That is, you should do a deep copy. If you look at what is being done for the other constructors (see their description under “Provide functions and constructors”) you’ll save yourself some work in creating the storage for the array in the object being initialized.

~Array2D: a destructor for a 2D array. It needs to free up the data from the actual array data, contained in ary. Hint: see and understand deleteAry(int** ary) that is provided to you.

Array2D&amp; operator=: assigns a 2D array to another 2D array. In the assignment a1 = a2; the storage of a1 data representing the actual array should be different than the storage of the data of the a2 array. That is, you should do a deep copy.

bool operator==: compares two 2D arrays for equality. Two 2D arrays are equal if they have the same number of rows and columns and all of their elements are equal. Otherwise they are not equal.

Array2D operator*: perform a 2D matrix multiply. Check for the arrays have dimensions that are compatible to being multiplied. Return an array filled with -1s that is the size of the this array if this is the case.

std::ostream&amp; operator&lt;&lt;: put the elements of the array represented by a Array2D on the output stream. The file output.txt shows how the array output should work.

int getNumRows( ), int getNumCols( ): getters that get the number of rows and columns of the array being represented.

Provided functions and constructors.

I have provided some functions and constructors for you, either because they are illustrative of useful tricks and techniques, or because they are not really central to operator overloading and there’s no reason for 100 of you to implement these over and over again. I have also provided the HW5.cpp file that contains the main function, which should not need changing.

Array2D::Array2D(int numR, int numC) : Array2D(numR, numC, 0, false): This constructor is used to create a 2DArray where the elements are initialized using default values, which in this case is to initialize each element to the value of its row index. It delegates to another constructor, called in the initializer list (shown in italics) to do the actual initialization of the array elements. Note that the constructor that is delegated to must be called in the initializer list.

Array2D::Array2D(int numR, int numC, int val) : Array2D(numR, numC, val, true): This constructor takes a default value (val) to initialize the array elements. Like the constructor above, it delegates to another constructor, called in the initializer list (shown in italics) to do the actual initialization of the array elements.

Array2D(Array2D::Array2D(int numR, int numC, int val, bool useVal): a private constructor called by the previous two constructors that actually initializes the array. By delegating to this constructor we don’t have to duplicate the code of setting up the storage for the 2D array.

int Array2D::operator( )(int row, int col) const and int&amp; Array2D::operator( )(int row, int col). C++ distinguishes between these based on whether the this pointer needs to be passed to a const parameter, or not. If this doesn’t need to be passed to a const parameter, the version that returns a reference to an int (int&amp;) is called, otherwise the one that returns an int is returned.

These functions are necessary because while we can overload the “[ ]” operator, there is no “[ ][ ]” operator in C++. “[ ][ ]” basically is the application of “[ ]” to an array of pointers, followed by application of another “[ ]” to what is returned by the first “[ ]”. Thus we use the “( )” operation to do 2D indexing, allowing us to write things like array(i,j) where array is a 2DArray object or reference.

Void Array2D(int** ary): These free up the storage so that you can see how to call deletes on arrays of pointers. It is private because it only works on the private ary variable whose layout should not be visible outside of 2DArray, so not inheriting class should really know how to override this. I’ve made it non-virtual so that even if a class that inherits from Array2D tries to override it, we won’t call that overriding function from code in the Array2D class.

What should be turned in?

The userid directory should be renamed with your userid, i.e., your Purdue login name. This directory should contain main.cpp, Array2D.cpp, Array2D.h. The graders should either be able to go into the userid directory and type g++ -std=c+11 *.cpp -o hw4 and compile your code, or you should supply a make file such that make compiles and executes your program. The directory should not contain .o files or executable files. Zip up this file (use .zip files, not .rar or .7z files, if at all possible, and if not at all possible let me know why) and turn it in to Brightspace.
