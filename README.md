puppet-add-sudoer
-----------------

Add multiple sudoers. Tested using [Puppetry](https://github.com/drogerschariot/Puppetry). 


Tested:
* Ubuntu 12.04
* Debian 7
* CentOS 6.4


#### Usage #####
<pre>
<code>
add_sudoer { 'username':
	ssh_key 	=> 'somesshpubkey',
	password	=> 'somesha512hash', 
	no_sudopass	=> true, # when you run sudo, you will not be prompted for a password
	$uid 		=> '555', 
	$bash  		=> '/bin/bash',
	$home  		=> '/home/foo'
</code>
</pre>
