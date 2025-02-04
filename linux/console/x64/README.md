# Encryptor-Console (Version 2.0.0)
Encrypt or decrypt files with Encryptor-Console. It is a terminal-based program. It accepts multiple files and folders separated by path separators (`:`) as input and performs operations recursively and concurrently. Additionally, it hides file names (not folder names) for better confidentiality. Encryption or decryption of drives is currently not supported but it can encrypt or decrypt all files inside a drive. It also supports command-line usage. Use `./Encryptor-Console --help` to view the help page.

---

## Usage
You can run `Encryptor-Console` from the terminal for live interaction or invoke it by passing command-line arguments.
* > ./Encryptor-Console
* > ./Encryptor-Console [options] --path [path1:path2:path3:...] --password mypassword

---

## Options:

* **--encrypt, -e**  
  > Encryption mode. Default choice.
  
* **--decrypt, -d**  
  > Decryption mode.
  
* **--path, -p**  
  > Paths to the files and folders. If the path to a folder is given, it performs operations recursively and concurrently.  
  > Multiple paths should be separated by the path separator (`:`).
  
* **--no-modify, -nm**  
  > Don't hide encrypted file names or don't retrieve decrypted file names.
  
* **--threads, -t**  
  > Thread count in the range [1, 10]. Default value = [5].
  
* **--password**  
  > Password used to encrypt or decrypt the file. Password length must be in the range of [5, 50].
  
* **--no-color, -nc**  
  > Suppress color outputs.
  
* **--help, -h**  
  > View this help page.

---

## Examples:
                                               
* **./Encryptor-Console -e --path path_to_the_file_or_folder -t 10 --password mypassword**  
  > Encrypts `path_to_the_file_or_folder` with password `"mypassword"` and [10] threads running concurrently.

* **./Encryptor-Console --password mypassword path_to_the_file_or_folder**  
  > Encrypts `path_to_the_file_or_folder` with password `"mypassword"` and [5] threads running concurrently.

---

## Requirements
* **Terminal**

---

## Note
- Please verify the file checksums (SHA-256) before using Encryptor.
