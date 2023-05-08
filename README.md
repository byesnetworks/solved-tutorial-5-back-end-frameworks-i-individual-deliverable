Download Link: https://assignmentchef.com/product/solved-tutorial-5-back-end-frameworks-i-individual-deliverable
<br>
<strong>Learning Outcomes:                                                                                                                </strong>

<ul>

 <li>Work with the Back-End framework/library of your choice (i.e., the one you have decided to use for your project).</li>

 <li>Understand how API calls are written in the Back-End framework/library you have chosen (i.e., Express.js or Flask).</li>

 <li>Work individually to create a simple API.</li>

</ul>

<strong>Instructions: </strong>

<ul>

 <li>Use the code shown in the tutorial video for <strong>GET API</strong>, the <strong>API</strong> returns a list of user objects, and add new methods for a <strong>POST</strong>, <strong>PUT</strong> and a new <strong>GET API</strong></li>

</ul>

GET : &lt;your_application_link&gt;/users

Sample Success Response :

{

message : “Users retrieved”,              success : true,       users : [{                    email : “<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="9efffcfddefffcfdb0fdff">[email protected]</a>”,             firstName : “ABC”,                  id : “5abf6783”

}, {

email : “<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="522a2b28122a2b287c3133">[email protected]</a>”, firstName: “XYZ”,

id : “5abf674563”

}]

}













–      The <strong>PUT API</strong> should be able to update <strong>email and/or firstname</strong> of an existing object in the list. The new email and firstname should be passed in the body of the request.

PUT – &lt;your_application_link&gt;/update/:id body data:

{ email : “<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="c3bbbab983bbbab9eda0a2">[email protected]</a>”, firstName: “XYZ”,

}

Sample Success Response :

{

message : “User updated”,     success : true

}

–      The <strong>POST API</strong> should add a <strong>New User Object</strong> to the list and <strong>generate an ID</strong> for the user. The object details should be passed in the body of the request.

POST – &lt;your_application_link&gt;/add body data:

{ email : “<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="5c2425261c242526723f3d">[email protected]</a>”, firstName: “XYZ”,

}

Sample Success Response:

{

message : “User added”,       success : true

}










–               Finally, a new <strong>GET API</strong> should be written, which should return a single user object given its username.

The username can be passed as a query or path parameter.

GET- &lt;your_application_link&gt;/user/:id

Sample Success Response :

{

success : true,         user : {

email : “<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="7008090a3008090a5e1311">[email protected]</a>”, firstName: “XYZ”,

id : “5abf674563”

}

}

<ul>

 <li><strong>No front-end is required for this tutorial. </strong></li>

</ul>

<strong>Consider failure responses for each request as well </strong>(e.g., 404, 400, 500 responses and appropriate json messages