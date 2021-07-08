# ideaFoundry
 
<p>This is an exercise in laying out HTML using Bootstrap 5.
It's non functional but I've added in id's so that it could be used as
a template in javascript to generate custom invoices.</p>

data handles

<strong>title bar: use this to set the unique invoice number in the tab text</strong><br>
var titleInvoiceNumber = document.getElementById('titleInvoiceNumber');

<strong>usage</strong><br>
titleInvoiceNumber.innerText = '19006';

<strong>Client number</strong><br>
var clientNumber = document.getElementById("clientNumber");

<strong>invoice Date</strong><br>
var clientNumber = document.getElementById("invoiceDate");

<strong>invoice Number</strong><br>
var clientNumber = document.getElementById("invoiceNumber");

<strong>client Name, and 2 address lines</strong><br>
var clientNumber = document.getElementById("clientName");<br>
var clientNumber = document.getElementById("clientAddress");<br>
var clientNumber = document.getElementById("clientAddress2");<br>


For the table items we can use the table row and append our data cells <br>
var invoiceTableBody = document.getElementById('invoiceTableBody');

<strong>usage</strong>
first make sure the table body is empty<br>
invoiceTableBody.innerHTML = "";

then append your row and data cells. For this example our data is in the following variables
let name = 'Design';
let service = 'Website Design';
let serviceCost = 60;
let numberOfServices = 10;
let serviceTotal = serviceCost * numberOfServices

now to append you can loop through adding as many of these as needed.
keep in mind that you should keep a running total of how many items are listed and their total
cost so we can populate the table footer

invoiceTableBody.innerHTML += `<tr><td>${name}</td><td>${service}</td><td>$${serviceCost}</td><td>${numberOfServices</td><td>$${serviceTotal}</td></tr>`;


Finally we have our table footer
there are three ids we can use here<br>

var subTotal = document.getElementById("subTotal");<br>
var tax = document.getElementById("taxRate"); <br>
var finalTotal = document.getElementById("finalTotal");<br>

for each of these we can modify them with the lines below. this is where we would use the
totals we gathered in the previous step.

subTotal.innerText = `$${itemSubTotal}` <br>
tax.innerText = `$${itemTax}` <br>
finalTotal.innerText = `$${itemFinalTotal}`
