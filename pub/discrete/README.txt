                       README.txt               (24 October 2008)
                       ==========

DISCLAIMER:  This software and its documentation are free and come "as is"
             with absolutely no guarantee and no support.


A. Preparing the executable program:

   (1) MS Windows: discrete-windows.exe should be ready to run in Step B.

   (2) Linux executable:
        gunzip  discrete-linux.gz
        chmod  755  discrete-linux

   (3) Other operating systems:
       Compile with a command like:
         f77  -o discrete  discrete.for
         (Warnings about incompatible actual and dummy arguments in H12 
          are normal and harmless.)



B. Test run with a command (on MS Windows from the Command Prompt window) like:
     discrete-windows  <discrete.in  >test.out


C. Notes on compilers:
   The following reportedly run correctly (despite occasional compiler 
                                           warnings due to the Fortran 66):
     (a) Intel Fortran on MS Windows or Linux;
     (b) g77 on Linux
     (c) Most Linux & UNIX compilers (but not NAG F90);
     (d) Apple (Absoft compiler);
     (e) VMS Fortran complier;

D. Documentation:
   Necessary documentation must be downloaded from http://s-provencher.com.


                                               Stephen Provencher, PhD
