# PSLIBRARY QUICK-HELP

<p align="justify"> To generate the pseudopotentials of <code>pslibrary</code> 
you need
the <code>ld1.x</code> code of the <a href="http://www.quantum-espresso.org">Quantum ESPRESSO (QE)</a> distribution (to compile it, type <code style="font-family:monospace;">./configure</code> and <code>make ld1</code> in the main QE directory). 
Download from the <a href="https://dalcorso.github.io/pslibrary">pslibrary home page</a> 
the file <code>pslibrary.version.tar.gz</code> (the last stable version is <code>1.0.0</code>). Put
the file in a directory
and unpack it with the command:</p>

```
tar -xzvf ./pslibrary.version.tar.gz
```
<p align="justify"> A directory, <code>pslibrary.version</code>, is created. 
Enter in this directory
and write the path of the main QE directory in the file <code>QE_path</code>.
To generate the <code>pz</code>, <code>pbe</code>, <code>rel-pz</code>, and <code>rel-pbe</code> pseudopotentials for all elements
just type</p>
```
./make_all_ps
```
<p align="justify"> To generate the pseudopotential of one element, open 
the file <code>make_ps</code> and substitute the string <code>'all'</code> with the name of the element
(<code>'Cu'</code>, <code>'H.'</code>, etc.) before typing 
<code>./make_all_ps</code>. To generate
the pseudopotentials for other functionals enter in the directory with the
functional name and type</p>
```
. ../make_ps 
```
The pseudopotentials are saved in the directory 
<code>dft/PSEUDOPOTENTIALS</code>, where
<code>dft</code> is the functional name.
For more information see the <code>AAREADME</code> file in the <code>pslibrary.version</code> directory.

Need help to choose the PP? Read <a href="http://dalcorso.github.io/pslibrary/PP_list.html">here</a>.

