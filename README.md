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


For the table items we will populate each item with a loop. first get the table row
var invoiceItemRow = document.getElementById('invoiceItemRow');
