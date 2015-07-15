# LogicBoard
This is a java console implementation of the LogicBoard project.
It's purpose is for proof of concept. 
Once completed it will be implemented as an application using GUI. 
This project focuses on the data structure to handle creation,edits, and saves of a logicBoard project.
All source code has been designed and implemented by Kyle Ferguson (Brogrammer Studios).


Sample of Console
Console Output of OneBitFullAdder class:
<table>
<th>One bit full adder</th>
    <tr>
        <td>A</td>
        <td>B</td>
        <td>Cin</td>
        <td>|</td>
        <td>Cout</td>
        <td>Sum</td>
    </tr>
    <tr>
        <td>0</td>
        <td>0</td>
        <td>0</td>
        <td>  </td>
        <td>0</td>
        <td>0</td>
    </tr>
        <td>0</td>
        <td>0</td>
        <td>1</td>
        <td>  </td>
        <td>0</td>
        <td>1</td>
    </tr>
        <td>0</td>
        <td>1</td>
        <td>0</td>
        <td>  </td>
        <td>0</td>
        <td>1</td>
    </tr>
        <td>0</td>
        <td>1</td>
        <td>1</td>
        <td>  </td>
        <td>1</td>
        <td>0</td>
    </tr>
        <td>1</td>
        <td>0</td>
        <td>0</td>
        <td>  </td>
        <td>0</td>
        <td>1</td>
    </tr>
        <td>1</td>
        <td>0</td>
        <td>1</td>
        <td>  </td>
        <td>1</td>
        <td>0</td>
    </tr>
        <td>1</td>
        <td>1</td>
        <td>0</td>
        <td>  </td>
        <td>1</td>
        <td>0</td>
    </tr>
        <td>1</td>
        <td>1</td>
        <td>1</td>
        <td>  </td>
        <td>1</td>
        <td>1</td>
    </tr>
</table>
Process finished with exit code 0

<h2>Update 1</h2>
    As of now a clean up and error catching process is being done on the data structure.
    Once done Logic blocking, object saving and cloning will be implemented. This will allow 
    for saving of LogicBoards (blocks) and when deserialized multiple copies can be made so you can
    have mulitple logic blocks with the same logic from the saved version althroughout any other logic board.

<h2>Update 2</h2>
    Alright as of now new exceptions have been created for certain error occurances in the data structure. 
    Clean up is as always underway. Also Designs for new functions are being made.(hint hint circuit 
    simplification tools :D). However as testing continues I have started designing some much needed
    functions to make building boards more intuitive based on some not so intuitive processes I 
    designed earlier. Logicboards can be saved and cloned. LogicBoards implemented into other logicboards
    now act as a gate object as they now implement the Gate interface. Logicboards also allow you to rename 
    it's system output gates gateID. This allows for more intuitive debugging for whatever user is creating! 
    Might add some addition features for that. This is probably the biggest update... mainly cause I have 
    been lazy and haven't been logging the commits made since update 1. In any case, feel free to look at 
    the code friends. Please notify me before using code, alot of time has been spent on this...also becuase
    it's far from done.
    
<h2>Update 3</h2>
    Hey what's up guys!? Back for another update to the source code. Alright so first off I totally did an 
    overhaul to the folder structure of the project. This makes it emensely better as the structure of the 
    program is more clear and easier to understand. Next up is the beginning of the implementation of a
    sort-of sub project. I started designing and implementing some code that should be able to parse a 
    boolean expression, build a binary tree from it, and finally, based on the structure of the tree,
    build a logic board from the expression. This class that does this can take as many expressions and
    build logic based on it with the same board. The drawback is that the boolean expression can only
    contain values of the BOARDS INITIAL INPUTS. Each boolean expression only yeilds one ouput. Say you
    have a board with inputs of A, B, C, and D. We want it to output (A'+B*C) and have another 
    output: (D*C*A). Well the answer is staring us in the face! We would simply add those two expressions
    to a BoardTree objects list of expressions! The reason this works is becuase a gate can theoretically
    ouput TO an infinite number of inputs. The next thing I am going to work on is testing, debugging, and 
    of course fixing this new implementation. The next thing I want to work on is a SMART parser that can
    correct small/simple errors in the expression passed before parsing.
    (adding spaces, checking parentheses, etc.) Well thats it for this update message, thanks for reading and
    following!
    
<h2>Update 3.5</h2>
    What's up world!? Mini Update time! So In the last update (just above) I talked about adding a feature 
    that allows a LogicBoard Object to be able to build itself based on n number of boolean expressions. 
    Well it works! I also added a feature that allows one to view the boolean expresion of each and every
    gate in a LogicBoard object. This allows one who builds the LogicBoard gate by gate, to view the 
    boolean expression as they go as well as when they complete the build! A lot of code was added but just
    does a lot of solving for the expression feature, that's why I'm just considering this a +0.5 update! 
    Have A good one fellow Brogrammers, I catch ya in the next update!

