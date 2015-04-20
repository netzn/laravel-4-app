
<h2>Reliam App</h2>


####


There needs to be a page that displays all accounts belonging to a specific organization.
Grab the ID of the organization and match that up with a search through the accounts table for matching organization integers in that table.

:: get all accounts where $organization == FUHU ::



:: get all instances where $organization == FUHU ::

display those matching 

Questions:

Use Case #1: Should I start implementing user auth into the app.  This way I could present different views for different users, i.e. allow the sys admin to add in an organization w/ AWS keys and hide that from support associates. 

Use Case #3: 


<h3>Requirements:</h3>

<i>For this first iteration lets just focus 
on these three entities:</i>

<ul>
<li>Organization: Create, Read and Update</li>
<li>Account: Create, Read and Update</li>
<li>Instance: List in table, and Read individually.</li>
</ul>

<i>Here are the most critical use cases:</i>

<strong>Use Case #1:</strong>

<p>As a sys admin I should be able to create an organization 
and provide the AWS API keys for an account. Upon creation, 
the system would call a python script to collect data. </p>

<blockquote>This may be a long operation, so we would
 need some dummy progress bar animation</blockquote>

<strong>Use Case #2:</strong>
<p>As a support associate I should be able to select an organization, 
and view all instances for all accounts of the selected organization. </p>

<p>The instances page would have a table 
containing the following fields : </p>

<ul>
	<li>[column_name] => [UI label]</li>
	<li>id   =>  label: Instance Id</li>
	<li>tags  =>  Tags       // Heads up. This will be JSON string</li>
	<li>_state  =>  State</li>
	<li>public_dns_name => Public DNS Name</li>
	<li>ip_address  =>  Public IP</li>             
	<li>private_dns_name  => Private DNS Name</li>
	<li>private_ip_address  => Private IP</li>
	<li>instance_type  =>  Instance Type</li>
	<li>region  =>  Region</li>
	<li>account_name ??? (this is low priority)</li>
</ul>


<strong>Use Case #3:</strong>
<p>As a support associate I should able click a 
“Refresh Button” in Account pages. 
<p>Under the hood a python script will be called 
and take care of syncing data</p>


<h2>Installing Laravel VM with Homestead &amp; Vagrant</h2>

<div><a href="http://laravel.com/docs/4.2/homestead">Installing Laravel on Homestead Tutorial</a></div>

<strong>Summary:</strong>
<ul>
<li>Install Composer</li>
<li>Install Laravel CLI Tool</li>
<li>Run: homestead up</li>
<li>Run: homestead ssh</li>
<li>Run: php artisan migrate</li>
<li>Run: php artisan db:seed</li>
</ul>








