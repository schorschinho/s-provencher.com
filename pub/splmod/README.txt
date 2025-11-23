                       README.txt                 (17 May 2002)
                       ==========

DISCLAIMER:  This software and its documentation is free and comes "as is"
             with absolutely no guarantee and no support.


A. Preparing the executable program:

   (1a) Linux executable (may refuse to run with some distributions):
        gunzip  splmod-linux.gz
        mv  splmod-linux  splmod
        chmod  755  splmod

   (1b) or: Suggested Linux compilation of splmod.for:
          g77  -o splmod  -fno-f2c  -ffast-math  -O  splmod.for

   (2) Other operating systems:
       Compile with a command like:
         f77  -o splmod  splmod.for


B. Test run with a command like:
     ./splmod  <splmod.in  >test.out

     (Some warnings about output conversion are normal.)


C. Notes on compilers:

   Most Fortran 77 & Fortran 90 compilers accept this Fortran 66 code 
     without change.  The following reportedly run correctly (despite 
     occasional compiler warnings due to the Fortran 66):
     (a) VMS;
     (b) Most Linux & UNIX compilers (but not NAG F90);
     (c) Apple (Absoft compiler);
     (d) Microsoft 16-bit MS-DOS compilers;
     (e) Digital Visual Fortran with Microsoft Windows;
     (f) WATCOM Fortran 77 with IBM OS/2 and Microsoft Windows & DOS;
     (g) Force 2.0 for Microsoft Windows (currently free download from 
           http://www.forceproject.hpg.ig.com.br);
     (h) LCC-Win32 Fortran for Microsoft Windows (currently free download 
           from http://www.cs.virginia.edu/~lcc-win32).

   It would be much easier to use the above compilers instead of the 
     following, which apparently would require tediously moving (Fortran 66) 
     Hollerith characters that were stored as INTEGER into CHARACTER types:
     (a) MS Powerstation and Lahey compilers with Microsoft Windows.

   Corrections or additions to the above lists would be welcome.


D. Documentation:
   Necessary doucumentation must be downloaded from http://s-provencher.com.


                                               Stephen Provencher, PhD
