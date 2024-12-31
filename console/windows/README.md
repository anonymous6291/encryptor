# Encryptor-Console
Encrypt or decrypt files with Encryptor-Console. Encryptor-Console is a terminal-based program.
Encryptor-Console accepts a single file or folder as input and performs operations recursively and concurrently.
It also hides your file's name (not folder's name) for better confidentiality.
Encryption or decryption of drives is currently not supported.
It also supports command-line usage. Use "Encryptor-Console --help" for viewing help page.
# Usage
You can run Encryptor-Console from terminal for live interaction or invoke by passing command-line arguments.

**Encryptor-Console [options] --path path_to_the_file_or_folder --password mypassword**
                                               
## Options :
* --encrypt , -e
  > Encryption mode. Default choice.
* --decrypt , -d
  > Decryption mode.
* --path , -p
  > Path to the file or folder. If path to folder is given then it performs operations recursively and concurrently.
* --threads , -t
  > Threads count in the range [1,10]. Default value = [5].
* --password
  > Password used to encrypt or decrypt the file. Password's length must be in the range of [5,50].
* --help , -h
  > To view this help page.
# Examples :
* Encryptor-Console
  > Live terminal based interaction.
* Encryptor-Console -e --path path_to_the_file_or_folder -t 10 --password mypassword      -
  > Encrypts path_to_the_file_or_folder with password "mypassword" and [10] threads running concurrently.
* Encryptor-Console -p path_to_the_file_or_folder --password mypassword
  > Encrypts path_to_the_file_or_folder with password "mypassword" and [5] threads running concurrently.
# Requirements
Only a terminal (Windows = [cmd,powershell,etc.]) is needed to run this program.
