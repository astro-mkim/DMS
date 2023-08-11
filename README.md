# DMS (Debris disks around Main sequence Stars)

=====================================================================================

 				 ------------------------------------------------
 				 DMS: Debris disks around Main-sequence Star code
				 ------------------------------------------------


				 author(s):         Minjae Kim
				 version : 	        Nov 2019
				 email(s):          mkim@astrophysik.uni-kiel.de



 Parts of this code are based on debris/modim code (Ertel et al. 2012; Ertel et al. 2011)



PLEASE NOTE: The code is STILL IN DEVELOPMENT and bugs may exist!
						 If you find one, please email me and specify.

You are free to use and extend this code.
But please write me and specify the use (modification) of this code.

For details, please refere to 

M. Kim, S. Wolf, T. Löhne, F. Kirchschlager, A.V. Krivov
(2018 A&A 618, A38, https://arxiv.org/abs/1806.02391)


- SPECIAL THANKS

With the very generous help of many people that find bugs and modify better way

• Steve Ertel
• Robert Brunngräber
• Florian Kirchschlager
• Sebastian Wolf
• Thomas Stuber


=====================================================================================

---------------------------------------------------------------------------------------
0. Documentation
---------------------------------------------------------------------------------------

a. DMS documentation will be released soon (Dec 2019)

---------------------------------------------------------------------------------------
1. Preparations
---------------------------------------------------------------------------------------

a. compiler
Intel Fortran compiler/gfortran should give the best performence.

b. optional
Python2/3 (matplotlib, numpy, astropy, and so on) are required for visualization.

---------------------------------------------------------------------------------------
2. You have to compile the code:
---------------------------------------------------------------------------------------
CMake is used for to handle dependencies, compiler options and to produce a
Makefile.
Go into the build folder, run cmake, run make to build the program:

> cd build
> cmake ..
> make

To remove all built files:

> make clean

---------------------------------------------------------------------------------------
3. Run the code:
---------------------------------------------------------------------------------------

> ./dms

Example inputs:

> ./dms < ../input_image
> ./dms < ../input_SED
> ./dms < "path/to/input-file"

---------------------------------------------------------------------------------------
4. Visualisation
---------------------------------------------------------------------------------------

prepared scripts are found in the sub folder "visualization".
Python2/3 with various modules, e.g., matplotlib, numpy, astropy, and so on, are required.


> cd visualization
> python3 radial_profiles.py
> python3 images.py
> python3 SED.py

Please change scripts by your own purpose.

Ascii text file can be converted into the fitsfile via ascii_to_fits.py, which is given in
same folder.


---------------------------------------------------------------------------------------
5. Various optical data
---------------------------------------------------------------------------------------

prepared various optical data are found in the sub folder "Optical data (Kim et al. 2019)".
For more information, please see Kim et al. 2019

Constraining the detectability of water ice in debris disks
M. Kim, S. Wolf, A. Potapov, H. Mutschke, C. Jäger (2019) A&A 629, A141
https://ui.adsabs.harvard.edu/abs/2019A\&A...629A.141K/abstract

If you want to use these brand new optical data, then please cite
Kim et al. 2019; Reinert et al. 2015; Haßner et al. 2016; Potapov et al. 2019a; Potapov et al. 2019b





If you have further problems in running the code, PLEASE do not hesitate to ask me.
