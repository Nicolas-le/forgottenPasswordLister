# Forgot your own password?
## Create your own password-bruteforce-list based on known letters.


Simple and small project that calculates all permutations by using already known letters. It builds all combinations with other printable ascii characters. Only reasonable for short passwords or a high number of known letters and if the possible password is random and therefore not existing in established wordlists. 
It also provides the possibility to remove characters that are definitly not a part of the password, f.ex. `&,%,?,..`

Possible situations: "aah damn I know my password was like 5 characters long and contained a k 1". 
This script calculates all possible passwords and writes them to a file, easy to use for bruteforcing.

Also useful to understand some basic things about password safety, f.ex. no standard passwords, length, use of various characters (some devices have predefined passwords that only consist of numbers).

### Usage:

`git clone https://github.com/Nicolas-le/forgottenPasswordLister.git`

`cd forgottenPasswordLister`

`python3 lister.py <known-letters> <password-length> <output-filename>`

### Example: 

`python3 lister.py ak1 5 pwList.txt`

#### to-do: 
* implement function to give pre-order of known letters and reduce permutation count
* optimize calculation time
* for now it's a simple "hardcore bruteforcer" --> add statistical frequencies of letters (maybe in passwords) and by this ignore some letters 



