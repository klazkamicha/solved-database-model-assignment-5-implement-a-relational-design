Download Link: https://assignmentchef.com/product/solved-database-model-assignment-5-implement-a-relational-design
<br>
The purpose of this assignment is to give you practice with creating database structure using SQL and using the INSERT command to add data.




write a MySQL script to create the database structures necessary for the table descriptions below.  Once you have created the tables, add INSERT statements to your script load the tables with the data provided below.  Submit your .sql file to Canvas.




Please keep in mind that you will need this database to complete assignment 8. Therefore, it is important that you create and populate the tables with the table definitions and sample data provided below.




Note: Some of the tables may seem to be missing columns that they might have in a real database (for example, an address and social security number in the Employee table).  This has been done to try to keep this assignment as short as possible.  You must adhere to the table definitions and data provided below to get full credit.




Table definition for Grant_Source table:

<table>

 <tbody>

  <tr>

   <td width="140"><strong>Grant_source</strong></td>

   <td width="113"></td>

   <td width="113"></td>

   <td width="113"></td>

   <td width="113"></td>

  </tr>

  <tr>

   <td width="140">grant_src</td>

   <td width="113">Char</td>

   <td width="113">30</td>

   <td width="113">PK</td>

   <td width="113"></td>

  </tr>

 </tbody>

</table>




Data for the Grant_source table:

<table>

 <tbody>

  <tr>

   <td width="193"><strong>grant_src</strong></td>

  </tr>

  <tr>

   <td width="193">NSF</td>

  </tr>

  <tr>

   <td width="193">Carnegie Foundation</td>

  </tr>

 </tbody>

</table>




Table definition for Grant table

<table width="631">

 <tbody>

  <tr>

   <td width="175"><strong>Grant_table</strong></td>

   <td colspan="4" width="457"></td>

  </tr>

  <tr>

   <td width="175">grant_numb</td>

   <td width="101">Char</td>

   <td width="101">3</td>

   <td width="101">PK</td>

   <td width="154"></td>

  </tr>

  <tr>

   <td width="175">grant_src</td>

   <td width="101">Char</td>

   <td width="101">30</td>

   <td width="101"></td>

   <td width="154">FKReferences Grant_source</td>

  </tr>

  <tr>

   <td width="175">total_amt</td>

   <td width="101">Numeric</td>

   <td width="101">10, 2</td>

   <td width="101"></td>

   <td width="154"></td>

  </tr>

  <tr>

   <td width="175">principal_researcher</td>

   <td width="101">Char</td>

   <td width="101">3</td>

   <td width="101"></td>

   <td width="154">FKReferences Employee (emp_numb)</td>

  </tr>

 </tbody>

</table>










Data for the Grant table:

<table width="631">

 <tbody>

  <tr>

   <td width="115"><strong>grant_numb</strong></td>

   <td width="186"><strong>source</strong></td>

   <td width="96"><strong>total_amt</strong></td>

   <td width="234"><strong>principal_researcher</strong></td>

  </tr>

  <tr>

   <td width="115">001</td>

   <td width="186">NSF</td>

   <td width="96">450000</td>

   <td width="234">001</td>

  </tr>

  <tr>

   <td width="115">002</td>

   <td width="186">Carnegie Foundation</td>

   <td width="96">30000</td>

   <td width="234">001</td>

  </tr>

  <tr>

   <td width="115">003</td>

   <td width="186">NSF</td>

   <td width="96">150000</td>

   <td width="234">002</td>

  </tr>

  <tr>

   <td width="115">004</td>

   <td width="186">NSF</td>

   <td width="96">75500</td>

   <td width="234">003</td>

  </tr>

  <tr>

   <td width="115">005</td>

   <td width="186">Carnegie Foundation</td>

   <td width="96">32750</td>

   <td width="234">004</td>

  </tr>

 </tbody>

</table>




Table definition for the Vendor table:

<table width="631">

 <tbody>

  <tr>

   <td width="139"><strong>Vendor</strong></td>

   <td colspan="4" width="492"></td>

  </tr>

  <tr>

   <td width="139">vendor_numb</td>

   <td width="97">Char</td>

   <td width="118">3</td>

   <td width="118">PK</td>

   <td width="159"></td>

  </tr>

  <tr>

   <td width="139">vendor_name</td>

   <td width="97">Char</td>

   <td width="118">40</td>

   <td width="118"></td>

   <td width="159"></td>

  </tr>

  <tr>

   <td width="139">vendor_street</td>

   <td width="97">Char</td>

   <td width="118">50</td>

   <td width="118"></td>

   <td width="159"></td>

  </tr>

  <tr>

   <td width="139">vendor_city</td>

   <td width="97">Char</td>

   <td width="118">20</td>

   <td width="118"></td>

   <td width="159"></td>

  </tr>

  <tr>

   <td width="139">vendor_state</td>

   <td width="97">Char</td>

   <td width="118">2</td>

   <td width="118"></td>

   <td width="159"></td>

  </tr>

  <tr>

   <td width="139">vendor_zip</td>

   <td width="97">Char</td>

   <td width="118">10</td>

   <td width="118"></td>

   <td width="159"></td>

  </tr>

  <tr>

   <td width="139">vendor_phone</td>

   <td width="97">Char</td>

   <td width="118">12</td>

   <td width="118"></td>

   <td width="159"></td>

  </tr>

 </tbody>

</table>




Data for the Vendor table:

<table width="625">

 <tbody>

  <tr>

   <td width="120"><strong>vendor_numb</strong></td>

   <td colspan="2" width="200"><strong>vendor_name</strong></td>

   <td colspan="2" width="306"><strong>vendor_street</strong></td>

  </tr>

  <tr>

   <td width="120"><strong>vendor_city</strong></td>

   <td width="92"><strong>vendor_</strong><strong>state</strong></td>

   <td width="108"><strong>vendor_zip</strong></td>

   <td width="153"><strong>vendor_phone</strong></td>

   <td width="153"></td>

  </tr>

  <tr>

   <td width="120">001</td>

   <td colspan="2" width="200">Archaeology Supply Co.</td>

   <td colspan="2" width="306">85 Northland Highway</td>

  </tr>

  <tr>

   <td width="120">Newtown</td>

   <td width="92">MA</td>

   <td width="108">02111</td>

   <td width="153">999-555-0211</td>

   <td width="153"></td>

  </tr>

  <tr>

   <td width="120">002</td>

   <td colspan="2" width="200">Westview Camping, Inc.</td>

   <td colspan="2" width="306">10876 Outer Ring Road</td>

  </tr>

  <tr>

   <td width="120">Westview</td>

   <td width="92">CA</td>

   <td width="108">96123</td>

   <td width="153">998-555-6123</td>

   <td width="153"></td>

  </tr>

  <tr>

   <td width="120">003</td>

   <td colspan="2" width="200">Charter Airlines</td>

   <td colspan="2" width="306">25 Airport Way</td>

  </tr>

  <tr>

   <td width="120">Oldtown</td>

   <td width="92">GA</td>

   <td width="108">42601</td>

   <td width="153">997-555-2601</td>

   <td width="153"></td>

  </tr>

  <tr>

   <td width="120">004</td>

   <td colspan="2" width="200">Digger’s Paradise</td>

   <td colspan="2" width="306">567 Hammondview</td>

  </tr>

  <tr>

   <td width="120">Eastview</td>

   <td width="92">TN</td>

   <td width="108">73109</td>

   <td width="153">996-555-3109</td>

   <td width="153"></td>

  </tr>

 </tbody>

</table>




Table definition for the Purchase table:

<table width="607">

 <tbody>

  <tr>

   <td width="118"><strong>Purchase</strong></td>

   <td colspan="4" width="489"></td>

  </tr>

  <tr>

   <td width="118">po_numb</td>

   <td width="118">Char</td>

   <td width="118">6</td>

   <td width="47">PK</td>

   <td width="206"></td>

  </tr>

  <tr>

   <td width="118">po_date</td>

   <td width="118">Date</td>

   <td width="118"></td>

   <td width="47"></td>

   <td width="206"></td>

  </tr>

  <tr>

   <td width="118">grant_numb</td>

   <td width="118">Char</td>

   <td width="118">3</td>

   <td width="47"></td>

   <td width="206">FKReferences Grant</td>

  </tr>

  <tr>

   <td width="118">vendor_numb</td>

   <td width="118">Char</td>

   <td width="118">3</td>

   <td width="47"></td>

   <td width="206">FKReferences Vendor</td>

  </tr>

 </tbody>

</table>










Data for the Purchase table:

<table>

 <tbody>

  <tr>

   <td width="148"><strong>po_numb</strong></td>

   <td width="148"><strong>po_date</strong></td>

   <td width="148"><strong>grant_numb</strong></td>

   <td width="148"><strong>vendor_numb</strong></td>

  </tr>

  <tr>

   <td width="148">000001</td>

   <td width="148">3-15-04</td>

   <td width="148">001</td>

   <td width="148">003</td>

  </tr>

  <tr>

   <td width="148">000002</td>

   <td width="148">3-21-04</td>

   <td width="148">001</td>

   <td width="148">002</td>

  </tr>

  <tr>

   <td width="148">000003</td>

   <td width="148">3-21-04</td>

   <td width="148">002</td>

   <td width="148">001</td>

  </tr>

  <tr>

   <td width="148">000004</td>

   <td width="148">3-25-04</td>

   <td width="148">004</td>

   <td width="148">001</td>

  </tr>

  <tr>

   <td width="148">000005</td>

   <td width="148">3-25-04</td>

   <td width="148">003</td>

   <td width="148">004</td>

  </tr>

  <tr>

   <td width="148">000006</td>

   <td width="148">4-2-04</td>

   <td width="148">005</td>

   <td width="148">004</td>

  </tr>

 </tbody>

</table>




Table definition for the Line_item table:

<table>

 <tbody>

  <tr>

   <td width="138"><strong>Line_item</strong></td>

   <td colspan="4" width="445"></td>

  </tr>

  <tr>

   <td width="138">po_numb</td>

   <td width="115">Char</td>

   <td width="113">6</td>

   <td width="47">PK</td>

   <td width="170">FKReferences Purchase</td>

  </tr>

  <tr>

   <td width="138">item_description</td>

   <td width="115">Char</td>

   <td width="113">30</td>

   <td width="47">PK</td>

   <td width="170"></td>

  </tr>

  <tr>

   <td width="138">cost_each</td>

   <td width="115">Numeric</td>

   <td width="113">8,2</td>

   <td width="47"></td>

   <td width="170"></td>

  </tr>

  <tr>

   <td width="138">quantity</td>

   <td width="115">Integer</td>

   <td width="113"></td>

   <td width="47"></td>

   <td width="170"></td>

  </tr>

 </tbody>

</table>




Data for the Line_item table:

<table>

 <tbody>

  <tr>

   <td width="91"><strong>po_numb</strong></td>

   <td width="270"><strong>item_description</strong></td>

   <td width="126"><strong>cost_each</strong></td>

   <td width="103"><strong>quantity</strong></td>

  </tr>

  <tr>

   <td width="91">000001</td>

   <td width="270">First class tickets to Mexico</td>

   <td width="126">2500.10</td>

   <td width="103">6</td>

  </tr>

  <tr>

   <td width="91">000002</td>

   <td width="270">6-man tent</td>

   <td width="126">109.00</td>

   <td width="103">4</td>

  </tr>

  <tr>

   <td width="91">000002</td>

   <td width="270">Dining canopy</td>

   <td width="126">209.95</td>

   <td width="103">2</td>

  </tr>

  <tr>

   <td width="91">000002</td>

   <td width="270">Mosquito netting</td>

   <td width="126">35.50</td>

   <td width="103">24</td>

  </tr>

  <tr>

   <td width="91">000002</td>

   <td width="270">Camp stools</td>

   <td width="126">18.50</td>

   <td width="103">24</td>

  </tr>

  <tr>

   <td width="91">000002</td>

   <td width="270">Fully-equipped camping kitchen</td>

   <td width="126">1500.95</td>

   <td width="103">2</td>

  </tr>

  <tr>

   <td width="91">000003</td>

   <td width="270">Brush, size 0</td>

   <td width="126">4.95</td>

   <td width="103">15</td>

  </tr>

  <tr>

   <td width="91">000003</td>

   <td width="270">Brush, size 2</td>

   <td width="126">5.95</td>

   <td width="103">15</td>

  </tr>

  <tr>

   <td width="91">000003</td>

   <td width="270">G-pick</td>

   <td width="126">15.80</td>

   <td width="103">15</td>

  </tr>

  <tr>

   <td width="91">000003</td>

   <td width="270">Shovel, size 0</td>

   <td width="126">21.95</td>

   <td width="103">15</td>

  </tr>

  <tr>

   <td width="91">000003</td>

   <td width="270">Dry specimen case, size S</td>

   <td width="126">7.50</td>

   <td width="103">100</td>

  </tr>

  <tr>

   <td width="91">000003</td>

   <td width="270">Dry specimen case, size M</td>

   <td width="126">12.50</td>

   <td width="103">75</td>

  </tr>

  <tr>

   <td width="91">000003</td>

   <td width="270">Dry specimen case, size L</td>

   <td width="126">19.95</td>

   <td width="103">25</td>

  </tr>

  <tr>

   <td width="91">000004</td>

   <td width="270">Sleeping bag</td>

   <td width="126">110.95</td>

   <td width="103">10</td>

  </tr>

  <tr>

   <td width="91">000004</td>

   <td width="270">2-man tent</td>

   <td width="126">185.95</td>

   <td width="103">5</td>

  </tr>

  <tr>

   <td width="91">000004</td>

   <td width="270">G-pick</td>

   <td width="126">15.80</td>

   <td width="103">20</td>

  </tr>

  <tr>

   <td width="91">000004</td>

   <td width="270">Shovel, size 0</td>

   <td width="126">21.95</td>

   <td width="103">10</td>

  </tr>

  <tr>

   <td width="91">000004</td>

   <td width="270">Brush, size 0</td>

   <td width="126">4.95</td>

   <td width="103">10</td>

  </tr>

  <tr>

   <td width="91">000004</td>

   <td width="270">Brush, size 1</td>

   <td width="126">6.95</td>

   <td width="103">10</td>

  </tr>

  <tr>

   <td width="91">000005</td>

   <td width="270">Twine, 1000 meters</td>

   <td width="126">17.50</td>

   <td width="103">5</td>

  </tr>

  <tr>

   <td width="91">000005</td>

   <td width="270">Broom, corn</td>

   <td width="126">12.50</td>

   <td width="103">3</td>

  </tr>

  <tr>

   <td width="91">000005</td>

   <td width="270">Canvas tent, one room, 20 x 15</td>

   <td width="126">609.00</td>

   <td width="103">2</td>

  </tr>

  <tr>

   <td width="91">000005</td>

   <td width="270">Folding table</td>

   <td width="126">125.95</td>

   <td width="103">15</td>

  </tr>

  <tr>

   <td width="91">000006</td>

   <td width="270">Chemical toilet</td>

   <td width="126">85.95</td>

   <td width="103">5</td>

  </tr>

  <tr>

   <td width="91">000006</td>

   <td width="270">Latrine tent, 5-stall</td>

   <td width="126">329.95</td>

   <td width="103">1</td>

  </tr>

  <tr>

   <td width="91">000006</td>

   <td width="270">Tissue for chemical toilets</td>

   <td width="126">1.25</td>

   <td width="103">100</td>

  </tr>

 </tbody>

</table>




Table Definition for the Dig table:

<table>

 <tbody>

  <tr>

   <td width="133"><strong>Dig</strong></td>

   <td colspan="4" width="457"></td>

  </tr>

  <tr>

   <td width="133">dig_numb</td>

   <td width="104">Char</td>

   <td width="118">3</td>

   <td width="61">PK</td>

   <td width="175"></td>

  </tr>

  <tr>

   <td width="133">grant_numb</td>

   <td width="104">Char</td>

   <td width="118">3</td>

   <td width="61"></td>

   <td width="175">FKReferences Grant</td>

  </tr>

  <tr>

   <td width="133">dig_description</td>

   <td width="104">Char</td>

   <td width="118">30</td>

   <td width="61"></td>

   <td width="175"></td>

  </tr>

  <tr>

   <td width="133">location</td>

   <td width="104">Char</td>

   <td width="118">30</td>

   <td width="61"></td>

   <td width="175"></td>

  </tr>

 </tbody>

</table>




Data for the Dig table:

<table>

 <tbody>

  <tr>

   <td width="97"><strong>dig_numb</strong></td>

   <td width="108"><strong>grant_numb</strong></td>

   <td width="238"><strong>dig_description</strong></td>

   <td width="148"><strong>location</strong></td>

  </tr>

  <tr>

   <td width="97">001</td>

   <td width="108">002</td>

   <td width="238">Excavating Eskimo ruins</td>

   <td width="148">Barrow, AK</td>

  </tr>

  <tr>

   <td width="97">002</td>

   <td width="108">001</td>

   <td width="238">Excavating a new pyramid</td>

   <td width="148">Giza, Egypt</td>

  </tr>

  <tr>

   <td width="97">003</td>

   <td width="108">003</td>

   <td width="238">Documenting cave paintings</td>

   <td width="148">Rural France</td>

  </tr>

  <tr>

   <td width="97">004</td>

   <td width="108">005</td>

   <td width="238">Excavating mammoth skeleton</td>

   <td width="148">Hyde Park, NY</td>

  </tr>

 </tbody>

</table>




Table definition for the Employee table:

<table>

 <tbody>

  <tr>

   <td width="118"><strong>Employee</strong></td>

   <td colspan="4" width="472"></td>

  </tr>

  <tr>

   <td width="118">emp_numb</td>

   <td width="93">Char</td>

   <td width="108">3</td>

   <td width="102">PK</td>

   <td width="169"></td>

  </tr>

  <tr>

   <td width="118">first_name</td>

   <td width="93">Char</td>

   <td width="108">15</td>

   <td width="102"></td>

   <td width="169"></td>

  </tr>

  <tr>

   <td width="118">last_name</td>

   <td width="93">Char</td>

   <td width="108">15</td>

   <td width="102"></td>

   <td width="169"></td>

  </tr>

  <tr>

   <td width="118">emp_phone</td>

   <td width="93">Char</td>

   <td width="108">12</td>

   <td width="102"></td>

   <td width="169"></td>

  </tr>

 </tbody>

</table>




Data for the Employee table:

<table>

 <tbody>

  <tr>

   <td width="148"><strong>emp_numb</strong></td>

   <td width="148"><strong>first_name</strong></td>

   <td width="148"><strong>last_name</strong></td>

   <td width="148"><strong>emp_phone</strong></td>

  </tr>

  <tr>

   <td width="148">001</td>

   <td width="148">Idaho</td>

   <td width="148">Smith</td>

   <td width="148">999-555-0001</td>

  </tr>

  <tr>

   <td width="148">002</td>

   <td width="148">Leslie</td>

   <td width="148">Lewis</td>

   <td width="148">999-555-0002</td>

  </tr>

  <tr>

   <td width="148">003</td>

   <td width="148">Indigo</td>

   <td width="148">Jones</td>

   <td width="148">999-555-0003</td>

  </tr>

  <tr>

   <td width="148">004</td>

   <td width="148">Jackrabbit</td>

   <td width="148">Johnson</td>

   <td width="148">999-555-0004</td>

  </tr>

  <tr>

   <td width="148">005</td>

   <td width="148">Big Cheese</td>

   <td width="148">Boss</td>

   <td width="148">999-555-0005</td>

  </tr>

  <tr>

   <td width="148">006</td>

   <td width="148">Marian</td>

   <td width="148">Librarian</td>

   <td width="148">999-555-0006</td>

  </tr>

  <tr>

   <td width="148">007</td>

   <td width="148">Stays In</td>

   <td width="148">Clerk</td>

   <td width="148">999-555-0007</td>

  </tr>

  <tr>

   <td width="148">008</td>

   <td width="148">Loves To</td>

   <td width="148">Dig</td>

   <td width="148">999-555-0008</td>

  </tr>

  <tr>

   <td width="148">009</td>

   <td width="148">Starving</td>

   <td width="148">GraduateStudent</td>

   <td width="148">999-555-0009</td>

  </tr>

  <tr>

   <td width="148">010</td>

   <td width="148">Poor</td>

   <td width="148">GraduateStudent</td>

   <td width="148">999-555-0010</td>

  </tr>

  <tr>

   <td width="148">011</td>

   <td width="148">He Knows</td>

   <td width="148">More</td>

   <td width="148">999-555-0011</td>

  </tr>

  <tr>

   <td width="148">012</td>

   <td width="148">She Knows</td>

   <td width="148">More</td>

   <td width="148">999-555-0012</td>

  </tr>

 </tbody>

</table>




Table definition for the Dig_assignment table:

<table>

 <tbody>

  <tr>

   <td width="132"><strong>Dig_assignment</strong></td>

   <td colspan="4" width="458"></td>

  </tr>

  <tr>

   <td width="132">dig_numb</td>

   <td width="114">Char</td>

   <td width="55">3</td>

   <td width="66">PK</td>

   <td width="223">FKReferences Dig</td>

  </tr>

  <tr>

   <td width="132">emp_numb</td>

   <td width="114">Char</td>

   <td width="55">3</td>

   <td width="66">PK</td>

   <td width="223">FKReferences Employee</td>

  </tr>

 </tbody>

</table>







Data for the Dig_assignment table

<table>

 <tbody>

  <tr>

   <td width="115"><strong>dig_numb</strong></td>

   <td width="120"><strong>emp_numb</strong></td>

  </tr>

  <tr>

   <td width="115">001</td>

   <td width="120">001</td>

  </tr>

  <tr>

   <td width="115">001</td>

   <td width="120">008</td>

  </tr>

  <tr>

   <td width="115">001</td>

   <td width="120">009</td>

  </tr>

  <tr>

   <td width="115">001</td>

   <td width="120">010</td>

  </tr>

  <tr>

   <td width="115">002</td>

   <td width="120">001</td>

  </tr>

  <tr>

   <td width="115">002</td>

   <td width="120">011</td>

  </tr>

  <tr>

   <td width="115">002</td>

   <td width="120">012</td>

  </tr>

  <tr>

   <td width="115">003</td>

   <td width="120">002</td>

  </tr>

  <tr>

   <td width="115">004</td>

   <td width="120">004</td>

  </tr>

  <tr>

   <td width="115">004</td>

   <td width="120">003</td>

  </tr>

  <tr>

   <td width="115">004</td>

   <td width="120">011</td>

  </tr>

  <tr>

   <td width="115">004</td>

   <td width="120">012</td>

  </tr>

 </tbody>

</table>


