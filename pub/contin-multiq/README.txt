                       README.txt                 (17 May 2002)
                       ==========

DISCLAIMER:  This software and its documentation is free and comes "as is"
             with absolutely no guarantee and no support.


A. Preparing the executable program:

   (1a) Linux executable (may refuse to run with some distributions):
        gunzip  contin-multiq-linux.gz
        mv  contin-multiq-linux  contin-multiq
        chmod  755  contin-multiq

   (1b) or: Suggested Linux compilation of contin-multiq.for:
          g77  -o contin-multiq  -fno-f2c  -ffast-math  -O  contin-multiq.for

   (2) Other operating systems:
       Compile with a command like:
         f77  -o contin-multiq  contin-multiq.for

         (Warnings about incompatible actual and dummy arguments in H12 
          are normal and harmless.)



B. Test run with a command like:
     ./contin-multiq  <contin-multiq.in  >test.out


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
     Hollerith characters that I stored as INTEGER into CHARACTER types:
     (a) MS Powerstation and Lahey compilers with Microsoft Windows.

   Corrections or additions to the above lists would be welcome.


D. Documentation:
   Necessary doucumentation must be downloaded from http://s-provencher.com.
   The only documentation specialized to contin-multiq is in the comments at
     the top of contin-multiq.for.


                                               Stephen Provencher, PhD
