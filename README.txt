floppy:
	FORTRAN 77 program to calculate how many floppies are needed to write a program, files,

        directories, etc to floppies (3.5in 1440K floppies)

usage:
        enter UNIT,COUNT

        units:
     		'B' BYTES

			'K' KB

			'M' MB

			'G' GB

        total KB is units * count

        ex: 'M', 76 means you are writing 76MB of data to floppies

  	'G' is for entertainment purposes mainly. You'd have to be insane to write even 1G of 
data to floppies

NOTE: this program does not take into consideration the space reserved 

for the MBR (Master Boot Record) so it may need a few extra floppies.

compile:

	Linux: just run compile.sh. It compiles and strips the binary. (requires gfortran)

	freeDOS: run C:\DEVEL\WATCOMF\OWSETENV.BAT (set the envirnment ) (requires WATCOMF)

			WFL C:\SRC\F77\FLOPPY.F (or whatever the path is to floppy.f will create floppy.exe)
