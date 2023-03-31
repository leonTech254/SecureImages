# SecureImages

This is a Python project that demonstrates how to encrypt and decrypt image files using the AES algorithm.

## Installation

<ul>
<li>Clone this repository:
<pre>
<code>
git clone git@github.com:leonTech254/SecureImages.git
</code>
</pre>
</li>
<li>Navigate to the project directory:
<pre>
<code> cd secure-images</code>
</pre>

</li>
<li>Install the required dependencies: 
<pre>
<code>
pip install -r requirements.txt
</code>
</pre>
</li>

</ul>

## Usage

### Encryption

<ol>
<li>
Run main.py
<pre>
<code>
python main.py
</code>
</pre>
<ul>
To change the image to be encrypted update the image path to match your pat <br>
"path/to/your/image"
<pre>
<code>
with open('./Images/leonLogo.png', 'rb') as infile:
</code>
</pre>
</ul>
</li>
</ol>

### Decryption

<ol>
<li>
open decrypt.py  file by default [after running the main.py file "output_image.enc"] will be generate on the same path and a The was used to encrypt the image will be printed on the terminal
</li>
<li>Copy the Key and update the key variable in  the decrypt.py file
<pre>
<code>
with open('output_image.enc', 'rb') as infile:
    iv = infile.read(BLOCK_SIZE)
    ciphertext = infile.read()
key = b'\x81\x07P\xe8\x11\x93\xee\xbf\xea,\x08]\xad\xc7A\x7f' #you will update the key here
</code>
</pre>
</li>
<li>Run the decrypt.py file and the plain image with decrypted_image.jpg will be generate
<pre>
<code>python decrypt.py</code>
</pre>

</li>
</ol>

## Developers

<ol>
<li>martinleontech23@gmail.com</li>
<li> wanguivalentine19@gmail.com</li>
</ol>
