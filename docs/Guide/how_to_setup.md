#

**Prerequisite**

Xampp

Clone this Repo directly into xampp/htdocs path.

**Front End**

Go to - application/config.php

Set - $config['base_url'] = 'http://example.com/' or 'https://example.com/'

Go to - application/database.php

Set -
'hostname' => 'localhost', (change required if needed)
'username' => '',
'password' => '',
'database' => '',

Go to - application/emailc.php

Set -

$config['$econfig'] = array('protocol' => 'smtp',

'smtp_host' => '', /* email gateway host /

'smtp_port' => 465,

'smtp_user' => '', / email gateway username /

'smtp_pass' => '', / email gateway password */

'wordwrap' => TRUE,

'charset' => 'utf-8');


**adminpanel**

Go to - application/adminpanel/config.php

Set - $config['base_url'] = 'http://example.com/adminpanel/' or 'https://example.com/adminpanel/'

Go to - application/adminpanel/constants.php

Set to - define('BASE_FRONT_URL', 'http://example.com/' or 'https://example.com/');

Go to - application/adminpanel/database.php

Set to -

'hostname' => 'localhost', (change required if needed)

'username' => '',

'password' => '',

'database' => '',


**[Click Here for Demo](https://www.youtube.com/watch?v=C0DF2A5ssk8)**