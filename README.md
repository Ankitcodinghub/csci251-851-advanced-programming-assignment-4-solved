# csci251-851-advanced-programming-assignment-4-solved
**TO GET THIS SOLUTION VISIT:** [CSCI251/851 Advanced Programming Assignment 4 Solved](https://www.ankitcodinghub.com/product/csci251-851advanced-programming-assignment-4-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;10583&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSCI251\/851 Advanced Programming  Assignment 4  Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
            5/5 - (3 votes)    </div>
    </div>
Gain experience developing programs using STL containers and inheritance.

<strong>On completion you should know how to:</strong>

<ul>
<li>Write C++ code using STL container class objects.</li>
<li>Use inheritance to facilitate programming with objects.</li>
<li>Gain experience writing and debugging O-O programs incrementally.</li>
</ul>
<strong>&nbsp;</strong>

<strong>Prerequisites: </strong>

This assignment involves writing a program to handle the billing of electricity, gas and phone accounts of a meter reading and billing company. Meter reading information on electricity, gas and phone usage is contained in the file “usage.txt”. Each record begins with the service type (i.e. elect, gas or phone) followed with customer details:

&nbsp;

<table width="189">
<tbody>
<tr>
<td width="189"><strong>BillingRecord </strong></td>
</tr>
<tr>
<td width="189">Supplier’s name

Customer’s&nbsp; name

Customer’s address

Account balance

Days since last reading
</td>
</tr>
</tbody>
</table>
&nbsp;

. . . and other usage information which depend on the service type:

&nbsp;

<table width="501">
<tbody>
<tr>
<td width="170"><strong>Electricity </strong></td>
<td width="161"><strong>Gas </strong></td>
<td width="170"><strong>Phone </strong></td>
</tr>
<tr>
<td width="170">Previous reading

Current reading

Rate 1

Rate 1 threshold

Rate 2

Supply charge
</td>
<td width="161">Previous reading

Current reading

Heating value

Rate

Supply charge
</td>
<td width="170">Number of local calls

Local call rate

Long distance call time

Long distance call rate

Line rental
</td>
</tr>
</tbody>
</table>
&nbsp;

This information is used to calculate the customer’s next bill. The processing of the billing records is complicated because some suppliers offer their customers discounts if they subscribe to more than one service from them. To solve this problem you are to use object oriented programming with inheritance to represent the different types of billing records. Polymorphism will also be used to allow all records to be processed efficiently in the one array.

&nbsp;

You should complete this assignment according to the following steps and demo &amp; submit your work according to the Submit and Demo instruction given at the end of this document. Each step is worth 2 marks and 2 marks is awarded for demoing your work on time in the lab. All code is to go in 5 files: B<strong>illRecord.h</strong>, B<strong>illRecord.cpp, BillSystem.h, BillSystem.cpp</strong> and <strong>main.cpp</strong>.

&nbsp;

&nbsp;

<h1>Billing System Design</h1>
The system is comprised of a BillSystem class object that own a vector of BillRecord objects in implemented in appropriately named files. The BillRecord class is a base class that has 3 derived classes for representing the 3 types of bills (elect. gas &amp; phone). The BillSystem has public functions for reading the data file into the BillRecord vector, processing the billing information and displaying the records on the screen. Some of the functions of the BillRecord class are overridden to handle the different types of data in the derived classes.

<strong>&nbsp;</strong>

<h1>Step 1&nbsp; (2 marks)</h1>
For step 1, get the BillRecord base class working. Examine the incomplete code in the provided files and complete the function definitions of class BillRecord and BillSystem so that the customer details (only) are read into each BillRecord of the vector BRecs from “usage.txt”. Then test that main() displays the first 10 customer details on the screen, as shown below. Note: don’t forget to delete the pointers in vector BRecs in the BillSystem destructor.

&nbsp;

<strong>&nbsp;# Service Supplier Customer&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Address&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;AccBal&nbsp; Days </strong>

<ul>
<li><strong>Phone Origin&nbsp;&nbsp; George Carter&nbsp; 24 Dingo St Exeter SA&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 49&nbsp;&nbsp;&nbsp; 28 </strong></li>
<li><strong>Gas EA&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Paul Scott&nbsp;&nbsp;&nbsp;&nbsp; 21 Beach Rd Barham NSW&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 98&nbsp;&nbsp;&nbsp; 30 </strong></li>
</ul>
<strong>&nbsp;“&nbsp; “&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; “&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; “&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; “ &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;“&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; “ </strong>

<strong>10 Gas&nbsp;&nbsp;&nbsp;&nbsp; EA&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;Carol Harris&nbsp;&nbsp; 67 Broke St Milton NSW&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 20.45&nbsp;&nbsp;&nbsp; 29 </strong>

&nbsp;

<h1>Step 2&nbsp; (2 marks)</h1>
Declare the derived BillRecord classes: ElectBillRecord, GasBillRecord and PhoneBillrecord in BillSystem.h. These classes inherit the base class BillRecord. Make sure you provide private data members for storing the relevant usage information shown on page 1. Change the BillRecord class’s private data member: AccountBalance and DaysSinceLastReading to protected to make them available to the derived classes. Also, make functions: ReadUsageInfo() and DisplayUsageInfo() into virtual functions so that they can be overridden by the base classes. See here:

https://www.geeksforgeeks.org/virtual-function-cpp/

&nbsp;

Now provide the derived classes with their versions of functions: ReadUsageInfo() and DisplayUsageInfo() to read and display their usage information appropriately.

&nbsp;

Modify ReadFile() in BillSystem.cpp so that it reads the service type and then allocates a

ElectBillRecord, GasBillRecord or PhoneBillrecord accordingly using the new operator. Then call their ReadCustDetails() and ReadUsageInfo() functions to have the data in the file read appropriately. You might have to work on the code in each ReadUsageInfo() function to get each derived class reading its file data correctly.

&nbsp;

When you complete this step run the main() again to display 5 records showing the Customer and usage info on the screen something like this:

&nbsp;

<strong># Service Supplier Customer&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Address&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; AccBal Days </strong>

<ul>
<li><strong>Phone Origin&nbsp;&nbsp; George Carter&nbsp; 53 Dingo St Exeter SA&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 49&nbsp;&nbsp; 28&nbsp;&nbsp;&nbsp; (LCalls: 283, 0.14&nbsp; DCalls: 245, 0.32&nbsp; Rental: 0.44)&nbsp;&nbsp; </strong></li>
<li><strong>Gas EA&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Paul Scott&nbsp;&nbsp;&nbsp;&nbsp; 84 Beach Rd Barham NSW&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 98&nbsp;&nbsp; 30 </strong></li>
</ul>
<strong>&nbsp;&nbsp; (Readings: 14148, 14224&nbsp; HV:38.40&nbsp; Rate: 0.039 SuppC: 0.56) </strong>

<ul>
<li><strong>Elect Alinta&nbsp;&nbsp; Brian Crowe&nbsp;&nbsp;&nbsp; 61 Beach Rd Hanwood WA&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 06&nbsp;&nbsp; 31&nbsp;&nbsp;&nbsp; (Readings: 113144, 113568&nbsp; R1: 0.28 R1Th: 535 R2: 0.30 SuppC: 0.86) </strong></li>
</ul>
<strong>&nbsp;</strong>

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; “&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; “&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; “&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; “&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; “&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;“ </strong>

&nbsp;

&nbsp;

<h1>Step 3&nbsp; (2 marks)</h1>
To win more customers Dodo and Alinta provide 15% and 20% discount, respectively, to all customers who subscribe to all three services from them. To deal with this add a protected data member to the BillRecord class named Discount and a public member function named SetDiscount(float d) for setting it. Also set Discount to one in the constructor. (Note: for 15% discount set Discount to 0.85. For 20% discount set Discount to 0.8.)

&nbsp;

There are various methods for finding which customers should have the discount applied. You can devise your own method if you wish but try to keep it efficient. The processing for this should be done in a public member function in the BillSystem class named CalDiscounts()..

&nbsp;

One suggestion for finding the discounted records is to use a multiset with a user defined

comparison object for ordering the BillRecord pointers. The comparison object should compare the BillRecords first by name and second by address. When all Dodo or Alinta records are inserted into this multiset, customers with the same name and address will be grouped and can be accessed with multiset functions: count(), lower_bound() and upper_bound(). (E.g. erase all BillRecord pointers with a count less than 3.) Once the discount pointers are found they can be dereferenced to set the discount appropriately. Test your code by uncommenting the “step-4” code in main() and print on the screen the number of discount customers Dodo and Alinta have.

&nbsp;

<h1>Step 4&nbsp; (2 marks)</h1>
Add two more public member functions to the BillSystem class named CalBills() and PrintReport(). Also add&nbsp; a public pure virtual function: UpdateBalance() in the BillRecord class and override this in the derived classes. UpdateBalance() should calculate the BillAmount and add this to the AccountBalance. The BillAmount is calculated as follows:

&nbsp;

<table width="584">
<tbody>
<tr>
<td width="76">Elect :</td>
<td width="508"><em>C = CrntReading – PrevReading;&nbsp;&nbsp; </em></td>
</tr>
<tr>
<td width="76"><em>&nbsp;</em></td>
<td width="508"><em>P = SuppyCharge * DaysSinceLastReading; </em></td>
</tr>
<tr>
<td width="76"><em>&nbsp;</em></td>
<td width="508"><em>If (C &lt;= R1Thld) BillAmt = (C * Rate1 + P) * Discount – AccBalance; </em></td>
</tr>
<tr>
<td width="76"><em>&nbsp;</em>

<em>&nbsp;</em>
</td>
<td width="508"><em>Else BillAmt = (R1Thld * Rate1 + (C – R1Thld) * Rate2 + P) * Discount – AccBalance;&nbsp; </em></td>
</tr>
<tr>
<td width="76">Gas : <em>&nbsp;</em></td>
<td width="508"><em>C = CrntReading – PrevReading;&nbsp;&nbsp; </em></td>
</tr>
<tr>
<td width="76"><em>&nbsp;</em></td>
<td width="508"><em>P = SuppyCharge * DaysSinceLastReading; </em></td>
</tr>
<tr>
<td width="76"><em>&nbsp;</em>

<em>&nbsp;</em>
</td>
<td width="508"><em>BillAmt = (C * HeatingValue * Rate) * Discount&nbsp; – AccBalance; </em></td>
</tr>
<tr>
<td width="76">Phone :</td>
<td width="508"><em>L = LocalCallRate * NumLocalCalls </em></td>
</tr>
<tr>
<td width="76"><em>&nbsp;</em></td>
<td width="508"><em>D = LDistCallRate * LDistCallTime&nbsp;&nbsp;&nbsp;&nbsp; </em></td>
</tr>
<tr>
<td width="76"><em>&nbsp;</em></td>
<td width="508"><em>P = LineRental * DaysSinceLastReading; </em></td>
</tr>
<tr>
<td width="76"><em>&nbsp;</em></td>
<td width="508"><em>BillAmt =&nbsp; (L + D + P) * Discount&nbsp; –&nbsp; AccBalance; </em></td>
</tr>
</tbody>
</table>
<strong>&nbsp;</strong>

<em>Note: the AccountBalance should be set to zero after the BillAmount is calculated. </em>

&nbsp;

PrintReport() should print the first 5 records similar to Step-1 with the “AccBal” and “Days” replaced with “BillAmt”. Also, print the names and addresses of all Dodo and Alinta customers who have discounts.

&nbsp;

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;</strong>

<strong>&nbsp;</strong>

<strong>Submit: </strong>

Submit your code files (and the output produced (copy &amp; paste) using the submit facility on UNIX as shown below:

&nbsp;

<strong>$ submit -u login -c CSCI251 –a4 main.cpp BillRecord.h BillRecord.cpp BillSystem.h BillSystem.cpp output.txt </strong>

<strong>&nbsp;</strong>

<strong>where ‘login’ is your UNIX login ID&nbsp; </strong>

Note: CSCI851 should also submit to –c CSCI251.

<strong>&nbsp;</strong>

<strong><u>You must demonstrate your program in the lab during your week 12 &amp; 13 lab classes to be</u></strong><strong> <u>awarded the demo marks (1 mark each). Work submitted and not demoed will be marked but</u> <u>there is no guarantee that it will be marked before the exam.</u> </strong>

<strong>&nbsp;</strong>

Deductions will be made for untidy work or for failing to comply with the submission instructions. Requests for alternative submission arrangements will only be considered before the due date. An extension of time for the assignment submission may be granted in certain circumstances.&nbsp; Any request for an extension of the submission deadline must be made to the Subject Coordinator before the submission deadline. Supporting documentation must accompany the request for any extension.&nbsp; Late assignment submissions without granted extension will be marked but the marks awarded will be reduced by 1 mark for each day late.&nbsp; Assignments will not be accepted if more than three days late.

&nbsp;
