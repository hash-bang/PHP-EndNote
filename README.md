PHP-EndNote
===========
Simple PHP library for reading and writing EndNote XML files.

**NOTE:** This library has now been incorporated into the [RefLib](https://github.com/hash-bang/RefLib) project.

This GitHub page is maintained so dependencies don't break.


Example: Read in EndNote XML
----------------------------

	require('endnote.php');
	$endnote = new PHPEndNote();
	$endnote->SetXMLFile('an-endnote-file.xml');

	print_r($endnote->refs); // Outputs all processed refs in an associative array


Example: Write EndNote XML
--------------------------

	require('endnote.php');
	$endnote = new PHPEndNote();
	$endnote->SetXMLFile('an-endnote-file.xml'); // Read in content (or populate $endnote->refs yourself)
	$endnote->OutputXML('EndNote File.xml'); // Output file to the browser
