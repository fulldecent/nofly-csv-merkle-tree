# nofly-csv-merkle-tree
A Merkle tree to privately confirm entries in NOFLY.csv and SELECTEE.csv


This is few single-page, offline web pages (HTML+JS) you can run to achieve a specific outcome.

**treeify.html** -- paste in NOFLY.csv or SELECTEE.csv and get the output file

- Input file is a csv file with columns: SID CLEARED LASTNAME FIRSTNAME MIDDLENAME TYPE DOB CITIZENSHIP PASSPORT/IDNUMBER MISC

- Output file is the same thing with more columns added: ROW_SHA256, ROW_PROOF, FIRSTNAME_MIDDLENAME_LISTNAME_PROOF

  - Make some privacy-preserving hash and SHA256 method

- Also there is a textfield outputting the root hash

**verify.html** -- paste in a ROW_PROOF and all row data // or paste in a FIRSTNAME_MIDDLENAME_LISTNAME_PROOF and the name fields and it is confirmed that the name is on the list

