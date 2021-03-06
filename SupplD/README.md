
Sage code for computing Dirichlet fundamental domains for the space of unlabeled networks on n vertices.

REQUIRED SOFTWARE:

Sage - http://www.sagemath.org/

lrslib - http://cgm.cs.mcgill.ca/~avis/C/lrs.html

SETUP:

This code is written in Python for the Sage mathematics software system. You will need to download, install, and configure the latest version of Sage, available at http://www.sagemath.org/.

The Polyhedra functions in Sage are able to make use of the following optional Sage package 'lrslib'. This is most easily installed within Sage using the following terminal command:

sage -i lrslib

Using this optional package will increase the speed these computations immensely, very roughly by a factor of 10.

RUNTIME:

The main file is 'fund_domain.sage'. To get started, change directories to the one containing this file. Enter the command

load('fund_domain.sage')

in the Sage environment. You will receive a prompt to set the global variable

n = your desired number of vertices

The global variable N = n choose 2. The global variable G=\Sigma_n will then be computed as a subgroup of the permutation group \Sigma_N. To construct a fundamental domain (for n=4, N=6) centered at the distinct vector l=[1,2,3,4,5,6.1], simply enter

F=fund_domain([1,2,3,4,5,6.1])[1]; F

F is a Sage polyhedron object representing a fundamental Dirichlet domain. Refer to the Sage documentation for the many available options for handling polyhedra:

http://doc.sagemath.org/html/en/reference/geometry/sage/geometry/polyhedron/constructor.html
