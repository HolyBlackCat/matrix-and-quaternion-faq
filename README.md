<sup><b>Disclaimer:</b> I (the owner of this repo) didn't write any of this. I merely found it on the net and converted to Markdown.</sup>

---

The Matrix and Quaternions FAQ
==============================

Version 1.21  30th November 2003
-------------------------------
Please mail feedback to <a href="mailto:matrix_faq@j3d.org">matrix_faq@j3d.org</a><br>
with a subject starting with <b> MATRIX-FAQ </b><br>
(otherwise my spam filter will simply kill your message).<br>
Any additional suggestions or related questions are welcome.<br>
Just send E-mail to the above address.<br>
The latest copy of this FAQ can be found at the following web page:<br>
    <a href="http://web.archive.org/web/20041029003853/http://web.archive.org/web/20041029003853/http://www.j3d.org/matrix_faq/matrfaq_latest.html">
http://www.j3d.org/matrix_faq/matrfaq_latest.html</a><br>
Feel free to distribute or copy this FAQ as you please.

Contributions
-------------

  <a href="#I1">Introduction I1</a>: <a href="mailto:steve@%28no-spam%29mred.bgm.link.com">Steve ?????</a><br>
  Correction to <a href="#Q55">Q55</a> until <a href="#Q59">Q59</a>:<br>
  <a href="mailto:andreas.junghanns@%28no-spam%29dcx.com">Andreas Junghanns</a><br>
  Correction to <a href="#Q50">Q50</a>: <a href="mailto:morten@%28no-spam%29innerloop.no">Morten Ofstad</a><br>
  Note to <a href="#Q39">Q39</a>: <a href="mailto:t.nuydens@%28no-spam%29vrcontext.com">Tom Nuydens</a><br>
  Corrections to <a href="#Q29">Q29</a> and <a href="#Q37">Q37</a>: <a href="mailto:eric@%28no-spam%29ee.pitt.edu">Eric Reiss</a><br>
  Clarification to <a href="#Q56">Q56</a>: <a href="mailto:murdoch@%28no-spam%29fisher.stats.uwo.ca">Duncan Murdoch</a><br>
  Clarification to <a href="#Q37">Q37</a>: <a href="mailto:avitzur@%28no-spam%29PacificT.com">Ron Avitzur</a><br>
  Correction to <a href="#Q1">Q1</a>: <a href="mailto:mona@%28no-spam%29ncmir.ucsd.edu">Mona Wong</a><br>
  Corrections to <a href="#Q36">Q36</a> and <a href="#Q37">Q37</a>: <a href="mailto:eric@%28no-spam%29ee.pitt.edu">Eric Reiss</a><br>
  Improvement to <a href="#Q34">Q34</a> and <a href="#Q38">Q38</a>: <a href="mailto:hplus-mail@%28no-spam%29mindcontrol.org">Jon Watte</a><br>
  Warning and alternative to <a href="#Q58">Q58</a> and <a href="#Q59">Q59</a>: <a href="mailto:PPedriana@%28no-spam%29maxis.com">Paul Pedriana</a><br>
  Correction (and optimization [Lee]) to <a href="#Q53">Q53</a>: <a href="mailto:ellieg@%28no-spam%29cableinet.co.uk">Eleanor Groundwater</a> and <a href="mailto:LeeMorgan@%28no-spam%29lee-morgan.net">Lee Morgan</a><br>
  Improvement to <a href="#Q39">Q39</a>: <a href="mailto:jhunpingco@%28no-spam%29yahoo.com">jhunpingco</a><br>
  Corrections to <a href="#Q11">Q11</a> and optimization to <a href="#Q12">Q12</a>: <a href="mailto:GDW33@%28no-spam%29student.canterbury.ac.nz">Gordon</a><br>
  Corrections to <a href="#Q54">Q54</a> to <a href="#Q60">Q60</a>: <a href="mailto:eleanorg@%28no-spam%29owl.co.uk">Eleanor Groundwater</a><br>
  Corrections and improvements to <a href="#Q23">Q23</a> and <a href="#Q24">Q24</a>: <a href="mailto:ben@%28no-spam%29exocortex.org">Ben Houston</a><br>
  Addition to <a href="#Q39">Q39</a>: <a href="mailto:hplus@%28no-spam%29mindcontrol.org">Jon Watte</a><br>
  Correction to <a href="#Q61">Q61</a>: <a href="mailto:adam@%28no-spam%29gimp.org">Adam D. Moss</a><br>
  Addition of <a href="#Q63">Q63</a>: <a href="mailto:cline@%28no-spam%29cs.ubc.ca">Mike Cline</a><br>
  Addition of <a href="#I2">I2</a>: <a href="mailto:jacob@%28no-spam%29marner.dk">Jacob Marner</a><br>
  Correction to <a href="#Q38">Q38</a> and inception of <a href="#I2">I2</a>: <a href="mailto:armuller@%28no-spam%29ira.uka.de">Armin M|ller</a><br>
  Addition of <a href="#Q60">Q60</a>: <a href="mailto:pfiguero@%28no-spam%29cs.ualberta.ca">Pablo Figueroa</a><br>
  Correntions and additions to <a href="#Q14">Q14</a>, <a href="#Q16">Q16</a>, <a href="#Q21">Q21</a> and <a href="#Q34">Q34</a>: <a href="mailto:tronster321@%28no-spam%29hotmail.com">Tronster Hartley</a><br>
  Correction to <a href="#Q12">Q12</a> and <a href="#Q54">Q54</a>: <a href="mailto:frankdj@%28no-spam%29mailhost.ph.tn.tudelft.nl">Frank DJ</a><br>
  Correction to <a href="#Q34">Q34</a>: <a href="mailto:robert.funnell@i%28no-spam%29mcgill.ca">Robert Funnell</a>


History
-------
I (Andreas) tried to find "<a href="mailto:hexapod@%28no-spam%29netcom.com">hexapod@(no-spam)netcom.com</a>" who seemed to have maintained<br>
this for a while, but the site at netcom.com doesn't exist anymore,<br>
emails bounce.  Since I (and colleques) wasted quite some time figuring out<br>
what was wrong with some of the algorithms given in the earlier versions of<br>
this document, I decided to correct it and put it back on the web.<br>
The formerly given sites for the location of these documents do<br>
not exist anymore:<br>
  ftp://ftp.netcom.com/pub/he/hexapod/index.html<br>
  http://www.glue.umd.edu/~rsrodger<br>
  Versions, dates and links to local copies (so you can compare):<br>
<a href="http://web.archive.org/web/20041029003853/http://web.archive.org/web/20041029003853/http://www.j3d.org/matrix_faq/matrfaq_1.02.html">matrfaq_1.02.html: Version 1.2  2nd September 1997</a><br>
<a href="http://web.archive.org/web/20041029003853/http://web.archive.org/web/20041029003853/http://www.j3d.org/matrix_faq/matrfaq_1.04.html">matrfaq_1.04.html: Version 1.4  26th December 1998</a><br>
<a href="http://web.archive.org/web/20041029003853/http://web.archive.org/web/20041029003853/http://www.j3d.org/matrix_faq/matrfaq_1.06.html">matrfaq_1.06.html: Version 1.6  30th September 2000</a><br>
<a href="http://web.archive.org/web/20041029003853/http://web.archive.org/web/20041029003853/http://www.j3d.org/matrix_faq/matrfaq_1.07.html">matrfaq_1.07.html: Version 1.7  20th December 2000</a><br>
<a href="http://web.archive.org/web/20041029003853/http://web.archive.org/web/20041029003853/http://www.j3d.org/matrix_faq/matrfaq_1.08.html">matrfaq_1.08.html: Version 1.8  21th December 2000</a><br>
<a href="http://web.archive.org/web/20041029003853/http://web.archive.org/web/20041029003853/http://www.j3d.org/matrix_faq/matrfaq_1.09.html">matrfaq_1.09.html: Version 1.9  16th January 2001</a><br>
<a href="http://web.archive.org/web/20041029003853/http://web.archive.org/web/20041029003853/http://www.j3d.org/matrix_faq/matrfaq_1.10.html">matrfaq_1.10.html: Version 1.10  30th January 2001</a><br>
<a href="http://web.archive.org/web/20041029003853/http://web.archive.org/web/20041029003853/http://www.j3d.org/matrix_faq/matrfaq_1.11.html">matrfaq_1.11.html: Version 1.11  9th February 2001</a><br>
<a href="http://web.archive.org/web/20041029003853/http://web.archive.org/web/20041029003853/http://www.j3d.org/matrix_faq/matrfaq_1.12.html">matrfaq_1.12.html: Version 1.12  26th March 2001</a><br>
<a href="http://web.archive.org/web/20041029003853/http://web.archive.org/web/20041029003853/http://www.j3d.org/matrix_faq/matrfaq_1.13.html">matrfaq_1.13.html: Version 1.13  20th July 2001</a><br>
<a href="http://web.archive.org/web/20041029003853/http://web.archive.org/web/20041029003853/http://www.j3d.org/matrix_faq/matrfaq_1.14.html">matrfaq_1.14.html: Version 1.14  17th August 2001</a><br>
<a href="http://web.archive.org/web/20041029003853/http://web.archive.org/web/20041029003853/http://www.j3d.org/matrix_faq/matrfaq_1.15.html">matrfaq_1.15.html: Version 1.15  20th August 2001</a><br>
<a href="http://web.archive.org/web/20041029003853/http://web.archive.org/web/20041029003853/http://www.j3d.org/matrix_faq/matrfaq_1.16.html">matrfaq_1.16.html: Version 1.16  2nd October 2001</a><br>
<a href="http://web.archive.org/web/20041029003853/http://web.archive.org/web/20041029003853/http://www.j3d.org/matrix_faq/matrfaq_1.17.html">matrfaq_1.17.html: Version 1.17  30th November 2001</a><br>
<a href="http://web.archive.org/web/20041029003853/http://web.archive.org/web/20041029003853/http://www.j3d.org/matrix_faq/matrfaq_1.18.html">matrfaq_1.18.html: Version 1.18  27th January 2002</a><br>
<a href="http://web.archive.org/web/20041029003853/http://web.archive.org/web/20041029003853/http://www.j3d.org/matrix_faq/matrfaq_1.19.html">matrfaq_1.19.html: Version 1.19  20th March 2002</a><br>
<a href="http://web.archive.org/web/20041029003853/http://web.archive.org/web/20041029003853/http://www.j3d.org/matrix_faq/matrfaq_1.20.html">matrfaq_1.20.html: Version 1.20  31st January 2002</a><br>
<a href="http://web.archive.org/web/20041029003853/http://web.archive.org/web/20041029003853/http://www.j3d.org/matrix_faq/matrfaq_1.21.html">matrfaq_1.21.html: Version 1.21  30th November 2003</a>


Please refrain from asking me math questions. I am only maintaining this FAQ<br>
and have very little knowledge about the subject. But, if you have a<br>
question that is not answered by this FAQ and later happen to find the<br>
answer and believe it to be relevant for this FAQ (or its readers), please<br>
send all relevant information, hopefully in a pre-digested form, to me to<br>
be included here. Thanks!<br>
If you prefer to appear as "anonymous" in the contributions list, let me<br>
know, otherwise I'll just put you down with whatever name I can gather from<br>
your email header.

Introduction
------------
<a href="#I1">I1.  Important note relating to OpenGL and this document</a><br>
<a href="#I2">I2.  Important note with respect to normalized inputs</a>

Questions
---------

BASICS
======
<a href="#Q1"> Q1. What is a matrix?</a><br>
<a href="#Q2"> Q2. What is the order of a matrix?</a><br>
<a href="#Q3"> Q3. How do I represent a matrix using the C/C++ programming languages?</a><br>
<a href="#Q4"> Q4. What are the advantages of using matrices?</a><br>
<a href="#Q5"> Q5. How do matrices relate to coordinate systems?</a>

ARITHMETIC
==========
<a href="#Q6"> Q6. What is the identity matrix?</a><br>
<a href="#Q7"> Q7. What is the major diagonal matrix of a matrix?</a><br>
<a href="#Q8"> Q8. What is the transpose of a matrix?</a><br>
<a href="#Q9"> Q9. How do I add two matrices together?</a><br>
<a href="#Q10">Q10. How do I subtract two matrices?</a><br>
<a href="#Q11">Q11. How do I multiply two matrices together?</a><br>
<a href="#Q12">Q12. How do I square or raise a matrix to a power?</a><br>
<a href="#Q13">Q13. How do I multiply one or more vectors by a matrix?</a>

DETERMINANTS AND INVERSES
=========================
<a href="#Q14">Q14. What is the determinant of a matrix?</a><br>
<a href="#Q15">Q15. How do I calculate the determinant of a matrix?</a><br>
<a href="#Q16">Q16. What are Isotropic and Anisotropic matrices?</a><br>
<a href="#Q17">Q17. What is the inverse of a matrix?</a><br>
<a href="#Q18">Q18. How do I calculate the inverse of an arbitary matrix?</a><br>
<a href="#Q19">Q19. How do I calculate the inverse of an identity matrix?</a><br>
<a href="#Q20">Q20. How do I calculate the inverse of a rotation matrix?</a><br>
<a href="#Q21">Q21. How do I calculate the inverse of a matrix using Kramer's rule?</a><br>
<a href="#Q22">Q22. How do I calculate the inverse of a 2x2 matrix?</a><br>
<a href="#Q23">Q23. How do I calculate the inverse of a 3x3 matrix?</a><br>
<a href="#Q24">Q24. How do I calculate the inverse of a 4x4 matrix?</a><br>
<a href="#Q25">Q25. How do I calculate the inverse of a matrix using linear equations?</a>

TRANSFORMS
==========
<a href="#Q26">Q26. What is a rotation matrix?</a><br>
<a href="#Q27">Q27. How do rotation matrices relate to coordinate systems?</a><br>
<a href="#Q28">Q28. How do I generate a rotation matrix in the X-axis?</a><br>
<a href="#Q29">Q29. How do I generate a rotation matrix in the Y-axis?</a><br>
<a href="#Q30">Q30. How do I generate a rotation matrix in the Z-axis?</a><br>
<a href="#Q31">Q31. What are Euler angles?</a><br>
<a href="#Q32">Q32. What are yaw, roll and pitch?</a><br>
<a href="#Q33">Q33. How do I combine rotation matrices?</a><br>
<a href="#Q34">Q34. What is Gimbal Lock?</a><br>
<a href="#Q35">Q35. What is the correct way to combine rotation matrices?</a><br>
<a href="#Q36">Q36. How do I generate a rotation matrix from Euler angles?</a><br>
<a href="#Q37">Q37. How do I generate Euler angles from a rotation matrix?</a><br>
<a href="#Q38">Q38. How do I generate a rotation matrix for a selected axis and angle?</a><br>
<a href="#Q39">Q39. How do I generate a rotation matrix to map one vector onto another?</a><br>
<a href="#Q40">Q40. How do I use matrices to convert between two coordinate systems?</a><br>
<a href="#Q41">Q41. What is a translation matrix?</a><br>
<a href="#Q42">Q42. What is a scaling matrix?</a><br>
<a href="#Q43">Q43. What is a shearing matrix?</a><br>
<a href="#Q44">Q44. How do I perform linear interpolation between two matrices?</a><br>
<a href="#Q45">Q45. How do I perform cubic interpolation between four matrices?</a><br>
<a href="#Q46">Q46. How can I render a matrix?</a>

QUATERNIONS
===========
<a href="#Q47">Q47.  What are quaternions?</a><br>
<a href="#Q48">Q48.  How do quaternions relate to 3D animation?</a><br>
<a href="#Q49">Q49.  How do I calculate the conjugate of a quaternion?</a><br>
<a href="#Q50">Q50.  How do I calculate the inverse of a quaternion?</a><br>
<a href="#Q51">Q51.  How do I calculate the magnitude of a quaternion?</a><br>
<a href="#Q52">Q52.  How do I normalise a quaternion?</a><br>
<a href="#Q53">Q53.  How do I multiply two quaternions together?</a><br>
<a href="#Q54">Q54.  How do I convert a quaternion to a rotation matrix?</a><br>
<a href="#Q55">Q55.  How do I convert a rotation matrix to a quaternion?</a><br>
<a href="#Q56">Q56.  How do I convert a rotation axis and angle to a quaternion?</a><br>
<a href="#Q57">Q57.  How do I convert a quaternion to a rotation axis and angle?</a><br>
<a href="#Q58">Q58.  How do I convert spherical rotation angles to a quaternion?</a><br>
<a href="#Q59">Q59.  How do I convert a quaternion to spherical rotation angles?</a><br>
<a href="#Q60">Q60.  How do I convert Euler rotation angles to a quaternion?</a><br>
<a href="#Q61">Q61.  How do I use quaternions to perform linear interpolation between matrices?</a><br>
<a href="#Q62">Q62.  How do I use quaternions to perform cubic interpolation between matrices?</a><br>
<a href="#Q63">Q63.  How do I use quaternions to rotate a vector?</a>

Introduction
------------

<a name="I1">I1</a>. Important note relating to OpenGl and this document
-------------------------------------------------------
  In this document (as in most math textbooks), all matrices are drawn<br>
  in the standard mathematical manner.  Unfortunately graphics libraries<br>
  like IrisGL, OpenGL and SGI's Performer all represent them with the<br>
  rows and columns swapped.<br>
  Hence, in this document you will see (for example) a 4x4 Translation<br>
  matrix represented as follows:

          | 1  0  0  X |
          |            |
          | 0  1  0  Y |
      M = |            |
          | 0  0  1  Z |
          |            |
          | 0  0  0  1 |

  In Performer (for example) this would be populated as follows:

    M[0][1] = M[0][2] = M[0][3] =
    M[1][0] = M[1][2] = M[1][3] =
    M[2][0] = M[2][1] = M[2][3] = 0 ;
    M[0][0] = M[1][1] = M[2][2] = m[3][3] = 1 ;
    M[3][0] = X ;
    M[3][1] = Y ;
    M[3][2] = Z ;

  ie, the matrix is stored like this:

          | M[0][0]  M[1][0]  M[2][0]  M[3][0] |
          |                                    |
          | M[0][1]  M[1][1]  M[2][1]  M[3][1] |
      M = |                                    |
          | M[0][2]  M[1][2]  M[2][2]  M[3][2] |
          |                                    |
          | M[0][3]  M[1][3]  M[2][3]  M[3][3] |

  OpenGL uses a one-dimensional array to store matrices - but fortunately,<br>
  the packing order results in the same layout of bytes in memory - so<br>
  taking the address of a pfMatrix and casting it to a float* will allow<br>
  you to pass it directly into routines like glLoadMatrixf.<br>
  In the code snippets scattered throughout this document, a one-dimensional<br>
  array is used to store a matrix. The ordering of the array elements is<br>
  transposed with respect to OpenGL.

  This Document                  OpenGL
        | 0  1  2  3  |            | 0  4  8  12 |
        |             |            |             |
        | 4  5  6  7  |            | 1  5  9  13 |
    M = |             |        M = |             |
        | 8  9  10 11 |            | 2  6  10 14 |
        |             |            |             |
        | 12 13 14 15 |            | 3  7  11 15 |

<a name="I2">I2</a>. Important note with respect to normalized inputs
----------------------------------------------------
  Note that most algorithms assume normalized inputs, such as vectors of<br>
  union length, or matrices with normalized main diagonal etc. It is possible,<br>
  and often enough the case, that algorithms (and the code snippets provided here)<br>
  work correctly with arbitrary inputs, but it is usually considered bad practise<br>
  (and you will pay in debugging time if you fail to observe this suggestion) to<br>
  rely on this property.


Answers
-------

BASICS
======
<a name="Q1">Q1</a>.  What is a matrix?
----------------------
  A matrix is a two dimensional array of numeric data, where each<br>
  row or column consists of one or more numeric values.<br>
  Arithmetic operations which can be performed with matrices include<br>
  addition, subtraction, multiplication and division.<br>
  The size of a matrix is defined in terms of the number of rows<br>
  and columns.<br>
  A matrix with M rows and N columns is defined as a MxN matrix.<br>
  Individual elements of the matrix are referenced using two index<br>
  values. Using mathematical notation these are usually assigned the<br>
  variables 'i' and 'j'. The order is row first, column second<br>
  For example, if a matrix M with order 4x4 exists, then the elements<br>
  of the matrix are indexed by the following row:column pairs:

        | 00 01 02 03 |
    M = | 10 11 12 13 |
        | 20 21 22 23 |
        | 30 31 32 33 |

  The element at the top right of the matrix has i=0 and j=3<br>
  This is referenced as follows:

    M    = M
     i,j    0,3

  In computer animation, the most commonly used matrices have either<br>
  2, 3 or 4 rows and columns. These are referred to as 2x2, 3x3 and 4x4<br>
  matrices respectively.<br>
  2x2 matrices are used to perform rotations, shears and other types<br>
  of image processing. General purpose NxN matrices can be used to<br>
  perform image processing functions such as convolution.<br>
  3x3 matrices are used to perform low-budget 3D animation. Operations<br>
  such as rotation and multiplication can be performed using matrix<br>
  operations, but perspective depth projection is performed using<br>
  standard optimised into pure divide operations.<br>
  4x4 matrices are used to perform high-end 3D animation. Operations<br>
  such as multiplication and perspective depth projection can be<br>
  performed using matrix mathematics.

<a name="Q2">Q2</a>.  What is the "order" of a matrix?
-------------------------------------
  The "order" of a matrix is another name for the size of the matrix.<br>
  A matrix with M rows and N columns is said to have order MxN.

<a name="Q3">Q3</a>.  How do I represent a matrix using the C/C++ programming languages?
-----------------------------------------------------------------------
  The simplest way of defining a matrix using the C/C++ programming<br>
  languages is to make use of the "typedef" keyword. Both 3x3 and 4x4<br>
  matrices may be defined in this way ie:

    typedef float MATRIX3[9];
    typedef float MATRIX4[16];

    Since each type of matrix has dimensions 3x3 and 4x4, this requires
  9 and 16 data elements respectively.<br>
  At first glance, the use of a single linear array of data values may<br>
  seem counter-intuitive. The use of two dimensional arrays may seem<br>
  more convenient ie.

    typedef float MATRIX3[3][3];
    typedef float MATRIX4[4][4];

  However, the use of two reference systems for each matrix element<br>
  very often leads to confusion. With mathemetics, the order is row<br>
  first (i), column second (j) ie.

     Mij

  Using C/C++, this becomes

     matrix[j][i]

     Using two dimensional arrays also incurs a CPU performance penalty in
  that C compilers will often make use of multiplication operations to<br>
  resolve array index operations.<br>
  So, it is more efficient to stick with linear arrays. However, one issue<br>
  still remains to be resolved. How is an two dimensional matrix mapped<br>
  onto a linear array? Since there are only two methods (row first/column<br>
  second or column first/row column).<br>
  The performance differences between the two are subtle. If all for-next<br>
  loops are unravelled, then there is very little difference in the<br>
  performance for operations such as matrix-matrix multiplication.<br>
  Using the C/C++ programming languages the linear ordering of each<br>
  matrix is as follows:

    mat[0]  = M        mat[3]  = M
               00                 03
    mat[12] = M        mat[15] = M
               30                 33
<br>

        |  0  1  2  3 |
        |             |              | 0 1 2 |
        |  4  5  6  7 |              |       |
    M = |             |          M = | 3 4 5 |
        |  8  9 10 11 |              |       |
        |             |              | 6 7 8 |
        | 12 13 14 15 |

<a name="Q4">Q4</a>.  What are the advantages of using matrices?
-----------------------------------------------
  One of the first questions asked about the use of matrices in computer<br>
  animation is why they should be used at all in the first place.<br>
  Intuitively, it would appear that the overhead of for-next loops and<br>
  matrix multiplication would slow down an application.<br>
  Arguments that resolve these objections can be pointed out. These include<br>
  the use of CPU registers to handle loop counters on-board data caches<br>
  to optimise memory accesses.<br>
  Advantages can also be pointed out. By following a mathematical approach<br>
  to defining 3D algorithms, it is possible to predict and plan the<br>
  design of a 3D animation system. Such mathematical approaches allow<br>
  for the implementation of character animation, spline curves and inverse<br>
  kinematics.<br>
  However, one objection that frequently comes up is that it would be<br>
  quicker to just multiply each pair of coordinates by the rotation<br>
  coefficients for that axis, rather than perform a full vector-matrix<br>
  multiplication.<br>
  ie. Rotation in X transforms Y and Z<br>
      Rotation in Y transforms X and Z
      Rotation in Z transforms X and Y
  The argument to this goes as follows:<br>
  Given a vertex V = (x,y,z), rotation angles (A,B and C) and translation<br>
  (D,E,F). A  the algorithm<br>
  is defined as follows:<br>

    sx = sin(A)             // Setup - only done once
    cx = cos(A)
    sy = sin(B)
    cy = cos(B)
    sz = sin(C)
    cz = cos(C)
    x1 =  x * cz +  y * sz  // Rotation of each vertex
    y1 =  y * cz -  x * sz
    z1 =  z
    x2 = x1 * cy + z1 * sy
    y2 = z1
    z2 = z1 * cy - x1 * sy
    x3 = x2
    y3 = y2 * cx + z1 * sx
    z3 = z2 * cx - x1 * sx
    xr = x3 + D             // Translation of each vertex
    yr = y3 + E
    zr = z3 + F

  Altogether, this algorithm will use the following amounts of processing<br>
  time:<br>

    Set-up                                 Per-vertex
    -------------------------              ------------------------
    6 trigonometric functions
    6 assignment operations.               12 assignment
                                           12 multiplication
                                            9 addition
    -------------------------              ------------------------

  Assume that the same operations is being performed using matrix<br>
  multiplication.<br>
  With a 4x4 matrix, the procesing time is used as follows:<br>

    Set-up                       Change    Per-vertex               Change
    --------------------------   ------    ------------------------ ------
    6  trigonometric functions    0                                  0
    18 assignment operation      -12        3  assignment           -9
    12 multiplication            +12        9  multiplication       -3
    6  subtraction               +6         6  addition             -3
    --------------------------   ------    ------------------------ ------

  Comparing the two tables, it can be seen that setting up a rotation<br>
  matrix costs at least 12 multiplication calculations and an extra<br>
  18 assignment calls.<br>
  However, while this may seem extravagant, the savings come from<br>
  processing each vertex. Using matrix multiplication, the savings made<br>
  from processing just 4 vertices, will outweigh the additional set-up<br>
  cost.

<a name="Q5">Q5</a>.  How do matrices relate to coordinate systems?
--------------------------------------------------
  With either 3x3 or 4x4 rotation, translation or shearing matrices, there<br>
  is a simple relationship between each matrix and the resulting coordinate<br>
  system.<br>
  The first three columns of the matrix define the direction vector of the<br>
  X, Y and Z axii respectively.<br>
  If a 4x4 matrix is defined as:

        | A B C D |
    M = | E F G H |
        | I J K L |
        | M N O P |

  Then the direction vector for each axis is as follows:

     X-axis = [ A E I ]
     Y-axis = [ B F J ]
     Z-axis = [ C G K ]

ARITHMETIC
==========

<a name="Q6">Q6</a>.  What is the identity matrix?
---------------------------------
  The identity matrix is matrix in which has an identical number of rows<br>
  and columns. Also, all the elements in which i=j are set one. All others<br>
  are set to zero. For example a 4x4 identity matrix is as follows:

        | 1 0 0 0 |
    M = | 0 1 0 0 |
        | 0 0 1 0 |
        | 0 0 0 1 |

<a name="Q7">Q7</a>.  What is the major diagonal of a matrix?
--------------------------------------------
  The major diagonal of a matrix is the set of elements where the<br>
  row number is equal to the column number ie.

    M   where i=j
     ij

  In the case of the identity matrix, only the elements on the major<br>
  diagonal are set to 1, while all others are set to 0.

<a name="Q8">Q8</a>.  What is the transpose of a matrix?
---------------------------------------
  The transpose of matrix is the matrix generated when every element in<br>
  the matrix is swapped with the opposite relative to the major diagonal<br>
  This can be expressed as the mathematical operation:

    M'   = M
      ij    ji

  However, this can only be performed if a matrix has an equal number<br>
  of rows and columns.<br>
  If the matrix M is defined as:

        |  0.707 -0.866 |
    M = |               |
        |  0.866  0.707 |

  Then the transpose is equal to:

        |  0.707  0.866 |
    T = |               |
        | -0.866  0.707 |

  If the matrix is a rotation matrix, then the transpose is guaranteed<br>
  to be the inverse of the matrix.

<a name="Q9">Q9</a>.  How do I add two matrices together?
----------------------------------------
  The rule of thumb with adding two matrices together is:<br>
    "add row and column to row and column"
  This can be expressed mathematically as:

    R   = M   + L
     ij    ij    ij

  However, both matrices must be identical in size.<br>
  For example, if the 2x2 matrix M is added with the 2x2 matrix L then<br>
  the result is as follow:

    R = M + L
        | A B C |   | J K L |
        |       |   |       |
      = | D E F | + | M N O |
        |       |   |       |
        | G H I |   | P Q R |

        | A+J B+K C+L |
        |             |
      = | D+M E+N F+O |
        |             |
        | G+P H+Q I+R |

<a name="Q10">Q10</a>.  How do I subtract two matrices?
-------------------------------------
  The rule of thumb with subtracting two matrices is:<br>
    "subtract row and column from row and column"
  This can be expressed mathematically as:

    R   = M   - L
     ij    ij    ij

  However, both matrices must be identical in size.<br>
  For example, if the 2x2 matrix L is subtracted from the 2x2 matrix M then<br>
  the result is as follows:

    R = M - L
        | A B C |   | J K L |
        |       |   |       |
      = | D E F | - | M N O |
        |       |   |       |
        | G H I |   | P Q R |

        | A-J B-K C-L |
        |             |
      = | D-M E-N F-O |
        |             |
        | G-P H-Q I-R |

<a name="Q11">Q11</a>. How do I multiply two matrices together?
---------------------------------------------
  The rule of thumb with multiplying two matrices together is:<br>
    "multiply row into column and sum the result".
  This can be expressed mathematically as:<br>

          n

          --
    R   = \   M   x L
     ij   /    ik    kj
          --
          k=1

  If the two matrices to be multiplied together have orders:

    M = AxB and L = CxD

  then the two values B and C must be identical.<br>
  Also, the resulting matrix has an order of AxD<br>
  Thus, it is possible to multiply a Nx4 matrix with a 4x4 matrix<br>
  but not the other way around.<br>
  For example, if the 4x4 matrix M is defined as:

        | A B C D |
    M = | E F G H |
        | I J K L |
        | M N O P |

  and a 4x2 matrix L is defined as:

    L = | Q R |
        | S T |
        | U V |
        | W X |

  then the size of the resulting matrix is 4x2. The resulting matrix<br>
  is defined as:

    R = M x L

        | A B C D |   | Q R |
      = | E F G H | x | S T |
        | I J K L |   | U V |
        | M N O P |   | W X |

        | AQ+BS+CU+DW  AR+BT+CV+DX |
      = | EQ+FS+GU+HW  ER+FT+GV+HX |
        | IQ+JS+KU+LW  IR+JT+KV+LX |
        | MQ+NS+OU+PW  MR+NT+OV+PX |

<a name="Q12">Q12</a>. How do I square or raise a matrix to a power?
--------------------------------------------------
  A matrix may be squared or even raised to an integer power. However<br>
  there are several restrictions. For all powers, the matrix must be<br>
  square, that is orthogonal and the same width and height<br>
  For example,

     -1
    M   is the inverse of the matrix

     0
    M   generates the identity matrix

     1
     M   leaves the matrix unchanged.

     2
    M   squares the matrix and

     3
    M   generates the cube of the matrix

    Raising a matrix to a power greater than one involves multiplying a matrix
  by itself a specific number of times.<br>
  For example,

     2
    M  = M . M

     3
    M  = M . M . M

  and so on.

  Raising the identity matrix to any power always generates the identity<br>
  matrix ie.

     n
    I  = I

  One can be bit faster using the following piece of code, note that m and i<br>
  are both getting changed:<br>

    m -> matrix to be raised to a power
    i -> power to raise matrix to
    a -> matrix that will contain the result
    I -> identity matrix
    / -> integer division (ie round down to nearest whole number)
    % -> integer remainder operation
    * -> matrix multiplication
<br>

    a=I
    while(i>0){
       if(i%2) a=a*m
       i=i/2
       m=m*m
    }

<a name="Q13">Q13</a>. How do I multiply one or more vectors by a matrix?
-------------------------------------------------------
  The best way to perform this task is to treat the list of vectors as<br>
  a single matrix, with each vector represented as a column vector.<br>
  If N vectors are to be multiplied by a 4x4 matrix, then they can be<br>
  treated as a single 4xN matrix:<br>
  If the matrix is defined as:

        | A B C D |
    M = | E F G H |
        | I J K L |
        | M N O P |

  and the list of vectors is defined as:

        | x1 x2 x3 x4 x5|
    V = | y1 y2 y3 y4 y5|
        | z1 z2 z3 z4 z5|
        | 1  1  1  1   1|

  Note that an additional row of constant terms is added to the vector<br>
  list, all of which are set to 1.0. In real life, this row does not<br>
  exist. It is simply used to make the orders of the matrix M and the<br>
  vector list V match.<br>
  Then the multiplication is performed as follows:

            M . V = V'

    | A B C D |   | x1 x2 x3 x4 x5 |   | A.x1+B.y1+C.z1+D A.x2+B.y2+C.z2+D ... |<br>
    | E F G H | . | y1 y2 y3 y4 y5 | = | E.x1+F.y1+G.z1+H E.x2+F.y2+G.z2+H ... |<br>
    | I J K L |   | z1 z2 y3 y4 z5 |   | I.x1+J.y1+K.z1+L I.x2+J.y2+K.z2+L ... |<br>
    | M N O P |   | 1  1  1  1  1  |   | M.x1+N.y1+O.z1+P M.x2+N.y2+O.z2+P ... |

  For each vector in the list there will be a total of 12 multiplication<br>
  16 addition and 1 division operation (for perspective).<br>
  If the matrix is known not to be a rotation or translation matrix then the<br>
  division operation can be skipped.

DETERMINANTS AND INVERSES
=========================

<a name="Q14">Q14</a>. What is the determinant of a matrix?
-----------------------------------------
  The determinant of a matrix is a floating point value which is used to<br>
  indicate whether the matrix has an inverse or not. If zero, then no<br>
  inverse exists. If non-zero, then an inverse exists.<br>
  As an example, consider a matrix consisting of a single element:

    M = [ 1 ].

  For a matrix of this size, the determinant is simply the value of the<br>
  single element.<br>
  Also, the inverse is simply the reciprocal of this single element:

     -1
    M   = [ 1 / M[0][0] ]

  If this single value is non-zero, then an inverse exists. In the case<br>
  of the identity matrix, this happens to be 1 / 1 or 1.0<br>
  However, if the value of this single element is zero, then the determinant<br>
  is also zero.

  Attempting to calculate the reciprocal of zero, generates a value of<br>
  infinity. This isn't permitted as far a matrices are concerned, so no<br>
  inverse of the matrix exists.<br>
  For an identity matrix, the determinant is always equal to one.<br>
  Any matrix with a determinant of 1.0 is said to be isotropic.<br>
  Thus all rotation matrices are said to be isotropic, since the<br>
  determinant is always equal to 1.0.<br>
  This can be proved as follows:

        | A B |   | cos X  -sin X |
    M = |     | = |               |
        | C D |   | sin X   cos X |

    D = AD - BC

    D = (cos X . cos X) -  (-sin X . sin X)

            2          2
    D = (cos X ) + (sin X)

            2       2
    But, cos X + sin X = 1

    Therefore,
    D = 1

<a name="Q15">Q15</a>. How do I calculate the determinant of a matrix?
----------------------------------------------------
  The determinant of a matrix is calculated using Kramer's rule, where<br>
  the value can be calculated by breaking the matrix into smaller<br>
  matrices.<br>
  For a 2x2 matrix M, the determinant D is calculated as follows:

        | A B |
    M = |     |
        | C D |

    D = AD - BC

  For 3x3 and 4x4 matrices, this is more complicated, but can be solved<br>
  by methods such as Kramer's Rule.

<a name="Q16">Q16</a>. What are Isotropic and Anisotropic matrices?
-------------------------------------------------
  An Isotropic matrix is one in which the sum of the squares of all<br>
  three rows or columns add up to one.<br>
  A matrix in which this is not the case, is said to be Anisotropic.<br>
  When 3x3 or 4x4 matrices are used to rotate and scale an object, it<br>
  is sometimes necessary to enlarge or shrink one axis more than the<br>
  others.<br>
  For example, with seismic surveys, it is convenient to enlarge the<br>
  Z-axis by a factor or 50 or more, while letting the X and Y axii<br>
  remain the same.<br>
  Another example is the implementation of "squash" and "stretch"<br>
  with character animation. When a character is hit by a heavy object<br>
  eg. an anvil, the desired effect is to make the character look stretched out<br>
  sideways and squashed vertically:<br>
  A suitable matrix would be as follows:

        |  2   0   0    0  |
    M = |  0   2   0    0  |
        |  0   0   0.5  0  |
        |  0   0   0    1  |

  However, there is problem looming ahead. While this matrix will cause<br>
  no problems with the transformation of vertex data, it will cause<br>
  problems with gouraud shading using outward normals.<br>
  Because the transformation stage is implemented using matrix<br>
  multiplication, both vertex data and outward normal data will be<br>
  multiplied with this matrix.<br>
  While this is not a problem with vertex data (it is the desired effect)<br>
  it causes a major headache with the outward normal data.<br>
  After raw multiplication, each outward normal will no longer be<br>
  normalised and consequently will affect other calculations such as<br>
  shading and back-face culling.

<a name="Q17">Q17</a>. What is the inverse of a matrix?
-------------------------------------
  Given a matrix M, then the inverse of that matrix, denoted as M<sup>-1</sup>  , is<br>
  the matrix which satisfies the following expression:

         -1
    M . M   = I

  where I is the identity matrix.<br>
  Thus, multiplying a matrix with its inverse will generate the identity<br>
  matrix. However, several requirements must be satisfied before the<br>
  inverse of a matrix can be calculated.<br>
  These include that the width and height of the matrix are identical and<br>
  that the determinant of the matrix is non-zero.<br>
  Calculating the inverse of a matrix is a task often performed in order<br>
  to implement inverse kinematics using spline curves.

<a name="Q18">Q18</a>. How do I calculate the inverse of an arbitary matrix?
----------------------------------------------------------
  Depending upon the size of the matrix, the calculation of the inverse<br>
  can be trivial or extremely complicated.<br>
  For example, the inverse of a 1x1 matrix is simply the reciprocal of<br>
  the single element:

  ie. M = | x |

  Then the inverse is defined as:

     -1   | 1 |
    M   = | - |
          | x |

  Solving 2x2 matrices and larger can be achieved by using Kramer's Rule<br>
  or by solving as a set of simultaneous equations.<br>
  However, in certain cases, such as identity or rotation matrices, the<br>
  inverse is already known or can be determined from taking the transpose<br>
  of the matrix.

<a name="Q19">Q19</a>. How do I calculate the inverse of an identity matrix?
----------------------------------------------------------
  Don't even bother. The inverse of an identity matrix is the identity<br>
  matrix. ie.

         -1
    I . I   = I

  Any identity matrix will always have a determinant of +1.

<a name="Q20">Q20</a>. How do I calculate the inverse of a rotation matrix?
---------------------------------------------------------
  Since a rotation matrix always generates a determinant of +1,<br>
  calculating the inverse is equivalent of calculating the transpose.<br>
  Alternatively, if the rotation angle is known, then the rotation<br>
  angle can be negated and used to calculate a new rotation matrix.

<a name="Q21">Q21</a>. How do I calculate the inverse of a matrix using Kramer's rule?
--------------------------------------------------------------------
  Given a 3x3 matrix M:

        | A B C |
        |       |
    M = | D E F |
        |       |
        | G H I |

  Then the determinant is calculated as follows:

             n
            ---
            \                           i
    det M = /   M    * submat    M  * -1
            ---  0,i         0,i
            i=1
  where

    submat   M defines the matrix composed of all rows and columns of M
          ij

  excluding row i and column j. submat<sub>ij</sub> may be called recursively.<br>

        | A B C |
    M = | D E F |  becomes submat   = | E F |
        | G H I |                11   | H I |

  If the determinant is non-zero then the inverse of the matrix exists.<br>
  In this case, the value of each matrix element is defined by:

     -1      1                            i+j
    M    = -----  *  det submat     M * -1
     j,i   det M               i,j

<a name="Q22">Q22</a>. How do I calculate the inverse of a 2x2 matrix?
----------------------------------------------------
  For a 2x2 matrix, the calculation is slightly harder. If the matrix is<br>
  defined as follows:

        | A B |
    M = |     |
        | C D |

  Then the determinant is defined as:

    det = AD - BC

  And the inverse is defined as:

     -1     1   |  D  -B  |
    M   =  ---  |         |
           det  | -C   A  |

  This can be proved using Kramer's rule. Given the matrix M:

        | A B |
    M = |     |
        | C D |

  Then the determinant is:

                           0                            1
    det =  M    * submat M    * -1 +  M    * submat M    * -1
            0,0           0,0          0,1           0,1

    <=>    M    * M    * 1         +  M    * M    * -1
            0,0    1,1                 0,1    1,0

    <=>    A  * D                  +  B    * C    * -1

    <=>    AD                      +  BC . -1

    <=>    AD - BC

    And the inverse is derived from:

     -1                      0+0      -1
    M    = det submat    * -1    <=> M    = M    *  1 <=> D
     0,0             0,0              0,0    1,1

     -1                      1+0      -1
    M    = det submat    * -1    <=> M    = M    * -1 <=> C * -1
     0,1             1,0              0,1    1,0

     -1                      0+1      -1
    M    = det submat    * -1    <=> M    = M    * -1 <=> B * -1
     1,0             0,1              1,0    0,1

     -1                      1+1      -1
    M    = det submat    * -1    <=> M    = M    *  1 <=> A
     1,1             1,1              1,1    0,0

     Then the inverse matrix is equal to:

     -1    1  |  D  -C |
    M   = --- |        |
          det | -B   A |

  Providing that the determinant is not zero.

<a name="Q23">Q23</a>. How do I calculate the inverse of a 3x3 matrix?
----------------------------------------------------
  For 3x3 matrices and larger, the inverse can be calculated by<br>
  either applying Kramer's rule or by solving as a set of linear<br>
  equations.<br>
  If Kramer's rule is applied to a matrix M:

        | A B C |
    M = | D E F |
        | G H I |

  then the determinant is calculated as follows:<br>
    det M = A * (EI - HF) - B * (DI - GF) + C * (DH - GE)

    Providing that the determinant is non-zero, then the inverse is
  calculated as:

     -1     1     |   EI-FH  -(BI-HC)   BF-EC  |
    M   = ----- . | -(DI-FG)   AI-GC  -(AF-DC) |
          det M   |   DH-GE  -(AH-GB)   AE-BD  |

  This can be implemented using a pair of 'C' functions:

    VFLOAT m3_det( MATRIX3 mat )
      {
      VFLOAT det;
      det = mat[0] * ( mat[4]*mat[8] - mat[7]*mat[5] )
          - mat[1] * ( mat[3]*mat[8] - mat[6]*mat[5] )
          + mat[2] * ( mat[3]*mat[7] - mat[6]*mat[4] );
      return( det );
      }

    int m3_inverse( MATRIX3 mr, MATRIX3 ma )
     {
     VFLOAT det = m3_det( ma );
     if ( fabs( det ) < 0.0005 )
       {

       m3_identity( mr );
       return(0);
       }

     mr[0] =    ma[4]*ma[8] - ma[5]*ma[7]   / det;
     mr[1] = -( ma[1]*ma[8] - ma[7]*ma[2] ) / det;
     mr[2] =    ma[1]*ma[5] - ma[4]*ma[2]   / det;
     mr[3] = -( ma[3]*ma[8] - ma[5]*ma[6] ) / det;
     mr[4] =    ma[0]*ma[8] - ma[6]*ma[2]   / det;
     mr[5] = -( ma[0]*ma[5] - ma[3]*ma[2] ) / det;
     mr[6] =    ma[3]*ma[7] - ma[6]*ma[4]   / det;
     mr[7] = -( ma[0]*ma[7] - ma[6]*ma[1] ) / det;
     mr[8] =    ma[0]*ma[4] - ma[1]*ma[3]   / det;
     return(1);
     }

<a name="Q24">Q24</a>. How do I calculate the inverse of a 4x4 matrix?
----------------------------------------------------
  As with 3x3 matrices, either Kramer's rule can be applied or the<br>
  matrix can be solved as a set of linear equations.<br>
  An efficient way is to make use of the existing 'C' functions defined<br>
  to calculate the determinant and inverse of a 3x3 matrix.<br>
  In order to implement Kramer's rule with 4x4 matrices, it is necessary<br>
  to determine individual sub-matrices. This is achieved by the following<br>
  routine:

    void m4_submat( MATRIX4 mr, MATRIX3 mb, int i, int j ) {
      int di, dj, si, sj;
      // loop through 3x3 submatrix
      for( di = 0; di < 3; di ++ ) {
        for( dj = 0; dj < 3; dj ++ ) {
          // map 3x3 element (destination) to 4x4 element (source)
          si = di + ( ( di >= i ) ? 1 : 0 );
          sj = dj + ( ( dj >= j ) ? 1 : 0 );
          // copy element
          mb[di * 3 + dj] = mr[si * 4 + sj];
        }
      }
    }

  The determinant of a 4x4 matrix can be calculated as follows:

    VFLOAT m4_det( MATRIX4 mr )
      {
      VFLOAT  det, result = 0, i = 1;
      MATRIX3 msub3;
      int     n;
      for ( n = 0; n < 4; n++, i *= -1 )
        {

        m4_submat( mr, msub3, 0, n );
        det     = m3_det( msub3 );
        result += mr[n] * det * i;
        }
      return( result );
      }

  And the inverse can be calculated as follows:

    int m4_inverse( MATRIX4 mr, MATRIX4 ma )
      {

      VFLOAT  mdet = m4_det( ma );
      MATRIX3 mtemp;
      int     i, j, sign;
      if ( fabs( mdet ) < 0.0005 )
        m4_identity( mr );
        return( 0 );
      for ( i = 0; i < 4; i++ )
        for ( j = 0; j < 4; j++ )
          {
          sign = 1 - ( (i +j) % 2 ) * 2;
          m4_submat( ma, mtemp, i, j );
          mr[i+j*4] = ( m3_det( mtemp ) * sign ) / mdet;
          }
      return( 1 );
      }

  Having a function that can calculate the inverse of any 4x4 matrix is<br>
  an incredibly useful tool. Application include being able to calculate<br>
  the base matrix for splines, inverse rotations and rearranging matrix<br>
  equations.

<a name="Q25">Q25</a>. How do I calculate the inverse of a matrix using linear equations?
-----------------------------------------------------------------------
  If a matrix M exists, such that:

         | A B C |
    M  = | D E F |
         | G H I |

  then the inverse exists:

         | P Q R |
    M' = | S T U |
         | V W X |

  and the following expression is valid:

                     -1
        M     .     M     = I

    | A B C |   | P Q R |   | 1 0 0 |
    | D E F | . | S T U | = | 0 1 0 |
    | G H I |   | V W X |   | 0 0 1 |

    The inverse can then be calculated through the solution as a set of
  linear equations ie.:

    | AP + BS + CV |   | 1 |   Column 0 (X)
    | DP + ES + FV | = | 0 |
    | GP + HS + IV |   | 0 |

    | AQ + BT + CW |   | 0 |   Column 1 (Y)
    | DQ + ET + FW | = | 1 |
    | GQ + HT + IW |   | 0 |

    | AR + BU + CX |   | 0 |   Column 2 (Z)
    | DR + EU + FX | = | 0 |
    | GR + HU + IX |   | 1 |

TRANSFORMS
==========

<a name="Q26">Q26</a>. What is a rotation matrix?
-------------------------------
  A rotation matrix is used to rotate a set of points within a<br>
  coordinate system. While the individual points are assigned new<br>
  coordinates, their relative distances do not change.<br>
  All rotations are defined using the trigonometric "sine" and "cosine"<br>
  functions.<br>
  For a two-dimensional coordinate system, the rotation matrix is as<br>
  follows:

    | cos(A)  -sin(A) |
    |                 |
    | sin(A)   cos(A) |

    With the rotation angle A set to zero, this generates the identity
  matrix:

        |  1  0 |
    I = |       |
        |  0  1 |

  If the rotation is set to +90 degrees, then the matrix is as follows:

        |  0 -1 |
    M = |       |
        |  1  0 |

  If the rotation is set to -90 degrees, then the matrix is as follows:

        |  0  1 |
    M = |       |
        | -1  0 |

  Negating the rotation angle is equivalent to generating the transpose<br>
  of the matrix.<br>
  If a rotation matrix is multiplied with its transpose, the result is<br>
  the identity matrix.

<a name="Q27">Q27</a>. How do rotation matrices relate to coordinate systems?
------------------------------------------------------
  Rotation matrices relate to coordinate systems in the following way.<br>
  Mathematical convention requires that a positive rotation angle<br>
  generates a clockwise rotation when looking from the origin towards<br>
  the positive end of the rotation axis.<br>
  Applying this rule, allows for the derivation of three Cartesian<br>
  rotation matrices. Consider a right-handed coordinate system. For each<br>
  rotation axis, look from the origin towards the positive end of the<br>
  selected axis. This generates the following three views:<br>

     +----------------------------------------+
     |                                        |
     |   X-axis       Y-axis        Z-axis    |
     |                                        |
     |                                        |
     |  ^ Y          ^ Z                Y ^   |
     |  |            |                    |   |
     |  |            |                    |   |
     |  |            |                    |   |
     |  |            |                    |   |
     |  O----> Z     O----> X      X <----O   |
     |                                        |
     +----------------------------------------+

  Since a positive rotation angle generates a clockwise rotation, it is
  possible to generate a set of coordinate mappings for each rotation.<br>
  For simplicity, a rotation of +90 will be considered:<br>
  Starting with the X-axis:

    ( 0, 1, 0 ) -> ( 0, 0, 1 )
    ( 0, 0, 1 ) -> ( 0,-1, 0 )
    ( 0,-1, 0 ) -> ( 0, 0,-1 )
    ( 0, 0,-1 ) -> ( 0, 1, 0 )

  These can be simplified to:

    X' =  X
    Y' = -Z
    Z' =  Y

  These can then be placed into a matrix:

         | 1  0       0     |
    Rx = | 0  cos A  -sin A |
         | 0  sin A   cos A |

  Doing the same for the Y-axis:

    ( 0, 0, 1) -> ( 1,0, 0)
    ( 1, 0, 0) -> ( 0,0,-1)
    ( 0, 0,-1) -> (-1,0, 0)
    (-1, 0, 0) -> ( 0,0, 1)

  These can be simplified to:

    X' = Z
    Y' = Y
    Z' = -X

  These can then be placed into a matrix:

         |  cos A   0   sin A  |
    Ry = |  0       1   0      |
         | -sin A   0   cos A  |

  And finally for the Z-axis:

    ( 0, 1, 0 ) -> ( -1,  0, 0 )
    (-1, 0, 0 ) -> (  0, -1, 0 )
    ( 0,-1, 0 ) -> (  1,  0, 0 )
    ( 1, 0, 0 ) -> (  0,  1, 0 )

  These can be simplified to:

    X' = -Y
    Y' =  X
    Z' =  Z

  Placing these into a matrix:

         |  cos A   -sin A    0  |
    Rz = |  sin A    cos A    0  |
         |  0        0        1  |

  These are the three basic rotation matrices used by OpenGL.

<a name="Q28">Q28</a>. How do I generate a rotation matrix in the X-axis?
-------------------------------------------------------
  Use the 4x4 matrix:

         |  1  0       0       0 |
     M = |  0  cos(A) -sin(A)  0 |
         |  0  sin(A)  cos(A)  0 |
         |  0  0       0       1 |

<a name="Q29">Q29</a>. How do I generate a rotation matrix in the Y-axis?
-------------------------------------------------------
  Use the 4x4 matrix:

         |  cos(A)  0   sin(A)  0 |
     M = |  0       1   0       0 |
         | -sin(A)  0   cos(A)  0 |
         |  0       0   0       1 |

<a name="Q30">Q30</a>. How do I generate a rotation matrix in the Z-axis?
-------------------------------------------------------
  Use the 4x4 matrix:

         |  cos(A)  -sin(A)   0   0 |
     M = |  sin(A)   cos(A)   0   0 |
         |  0        0        1   0 |
         |  0        0        0   1 |

<a name="Q31">Q31</a>. What are Euler angles?
---------------------------
  Euler angles are the name given to the set of rotation angles which<br>
  specify the rotation in each of the X, Y and Z rotation axii.<br>
  These are specfied in vector format eg. |x y z| and can be stored<br>
  as a VECTOR data structure.<br>
  For example, the set

    | 0  0  0 |

  will always generate the identity matrix.<br>
  Other angles are represented as follows:

    | 90 0  0 | is a rotation of +90 degrees in the X-axis.
    | 0 90  0 | is a rotation of +90 degrees in the Y-axis and
    | 0  0 90 | is a rotation of +90 degrees in the Z-axis.

  Euler angles can be represented using a single vector data structure.

<a name="Q32">Q32</a>. What are Yaw, Roll and Pitch?
----------------------------------
  Yaw, Roll and Pitch are aeronautical terms for rotation using the<br>
  Euclidean coordinate system (Euler angles), relative to the local<br>
  coordinate system of an aeroplane.<br>
  Imagine you are viewing an aeroplane from above and from directly behind.<br>
  The Z-axis is lined up with the tail and nose of the aeroplane.<br>
  The X-axis runs from the tip of the left wing to the tip of the right<br>
  wing.<br>
  The Y axis points straight up from the ground.<br>
  Pitch then becomes rotation in the X-axis, Yaw becomes rotation in the<br>
  Y-axis and Roll becomes rotation in the Z-axis.

<a name="Q33">Q33</a>. How do I combine rotation matrices?
----------------------------------------
  Rotation matrices are combined together using matrix multiplication.<br>
  As a result, the order of multiplication is very important.

<a name="Q34">Q34</a>. What is Gimbal lock?
-------------------------
  Gimbal lock is the name given to a problem that occurs with the use of<br>
  Euler angles. Because the final rotation matrix depends on the order<br>
  of multiplication, it is sometimes the case that the rotation in one<br>
  axis will be mapped onto another rotation axis.<br>
  Even worse, it may become impossible to rotate an object in a desired<br>
  axis. This is called Gimbal lock.<br>
  For example, assume that an object is being rotated in the order Z,Y,X<br>
  and that the rotation in the Y-axis is 90 degrees.<br>
  In this case, rotation in the Z-axis is performed first and therefore<br>
  correctly. The Y-axis is also rotated correctly. However, after<br>
  rotation in the Y axis, the X-axis is rotated onto the Z-axis.<br>
  Thus, any rotation in the X-axis actually rotates the object in the<br>
  Z-axis. Even worse, it becomes impossible to rotate the object in the X-axis.<br>
  A convenient solution to this problem is to make use of Quaternions.

<a name="Q35">Q35</a>. What is the correct way to combine rotation matrices?
----------------------------------------------------------
  Really, there is no "correct way" of combining rotation matrices.<br>
  However, in order to be able to predict the result of combining<br>
  matrices together, some organisation is required. This is also<br>
  necessary if a full 3D matrix library is to be built.<br>
  The simplest way to rotate an object is to multiply the matrices<br>
  using the order:

    M = X.Y.Z

  where M is the final rotation matrix, and X,Y,Z are the individual<br>
  rotation matrices. This defines a rotation in the X-axis (pitch) first,<br>
  followed by the Y-axis (yaw) and a final rotation in the Z-axis (roll).<br>
  However, whenever the view from the camera viewpoint is being<br>
  evaluated, then the order and signs of the rotation is reversed.<br>
  For example, if you are standing up, and turn to your left, everything<br>
  in your field of view appears to move towards the right.<br>
  However, someone else facing you will say that you turned towards their<br>
  right.<br>
  Thus the view from the camera is modelled using the order:

    M = -Z.-Y.-X

  This is the inverse (or transpose) of the rotation matrix generated<br>
  if the camera were being rendered as another object.

<a name="Q36">Q36</a>. How do I generate a rotation matrix from Euler angles?
-----------------------------------------------------------
  At first glance, the most obvious method to generate a rotation matrix<br>
  from a set of Euler angles is to generate each matrix individually and<br>
  multiply all three together ie.

    m3_rotx( mat_x,     vec -> angle_x );
    m3_roty( mat_y,     vec -> angle_y );
    m3_rotz( mat_z,     vec -> angle_z );
    m3_mult( mat_tmp,   mat_z, mat_y   );
    m3_mult( mat_final, mat_tmp, mat_x );

  This set of calls could be placed in a separate routine eg.

    m3_fromeuler( MATRIX *mat_final, VECTOR3 *euler )

  However, to perform this sequence of calls is very wasteful in terms<br>
  of processing time. Given that each 4x4 rotation matrix is guaranteed<br>
  to have 10 elements with value zero (0), 2 elements with value one (1)<br>
  and four others of arbitary value, over 75% of every matrix operation<br>
  is wasted. This does not include the set up and initialisation of each<br>
  matrix.<br>
  Altogether, over 75% of all matrix operations are spent processing<br>
  arithmetic expressions which lead to either zero or one.<br>
  A more efficient way must be found. Fortunately, there is another way<br>
  of determining the final resulting matrix.<br>
  If all three matrices are combined in algebraic format, the following<br>
  expression is defined:

    M = X.Y.Z

  where M is the final matrix,<br>
        X is the rotation matrix for the X-axis,
        Y is the rotation matrix for the Y-axis,
        Z is the rotation matrix for the Z-axis.

  Expanding into rotation matrices in algebraic format gives:

         |  1  0  0 |
    X  = |  0  A -B |
         |  0  B  A |

         |  C  0  D |
    Y  = |  0  1  0 |
         | -D  0  C |

         |  E -F  0 |
    Z  = |  F  E  0 |
         |  0  0  1 |

  where A,B are the cosine and sine of the X-axis rotation axis,<br>
        C,D are the cosine and sine of the Y-axis rotation axis,
        E,F are the cosine and sine of the Z-axis rotation axis.

  Then the expression:

    M  = X.Y.Z

  can be split into two matrix multiplications:

    M' = X.Y
    M  = M'.Z

  Evaluating M' first:

    M' = X.Y

         | 1  0  0 |   | C  0  D |
    M' = | 0  A -B | . | 0  1  0 |
         | 0  B  A |   |-D  0  C |

         | 1.C + 0.0 +  0.-D   1.0 + 0.1 +  0.0   1.D + 0.0 +  0.C |
    M' = | 0.C + A.0 + -B.-D   0.0 + A.1 + -B.0   0.D + A.0 + -B.C |
         | 0.C + B.0 +  A.-D   0.0 + B.1 +  A.0   0.D + B.0 +  A.C |

  Simplifying M' gives:

         |  C     0   D   |
    M' = |  B.D   A  -B.C |
         | -A.D   B   A.C |

         Evaluating M gives:

    M  = M'.Z

         |  C   0   D  |   | E -F  0 |
    M  = |  BD  A  -BC | . | F  E  0 |
         | -AD  B   AC |   | 0  0  1 |

         |   C.E + 0.F +   D.0    C.-F + 0.E +  D.0     C.0 + 0.0 +   D.1 |
    M  = |  BD.E + A.F + -BC.0   BD.-F + A.E + -BC.0   BD.0 + A.0 + -BC.1 |
         | -AD.E + B.F +  AC.0  -AD.-F + B.E +  AC.0  -AD.0 + 0.0 +  AC.1 |

  Simplifying M gives a 3x3 matrix:

         |  CE      -CF       D  |
    M  = |  BDE+AF  -BDF+AE  -BC |
         | -ADE+BF   ADF+BE   AC |

  This is the final rotation matrix. As a 4x4 matrix this is:

         |  CE      -CF       D   0 |
    M  = |  BDE+AF  -BDF+AE  -BC  0 |
         | -ADE+BF   ADF+BE   AC  0 |
         |  0        0        0   1 |

  The individual values of A,B,C,D,E and F are evaluated first. Also, the<br>
  values of BD and AD are also evaluated since they occur more than once.<br>
  Thus, the final algorithm is as follows:

    A       = cos(angle_x);
    B       = sin(angle_x);
    C       = cos(angle_y);
    D       = sin(angle_y);
    E       = cos(angle_z);
    F       = sin(angle_z);
    AD      =   A * D;
    BD      =   B * D;
    mat[0]  =   C * E;
    mat[1]  =  -C * F;
    mat[2]  =   D;

    mat[4]  =  BD * E + A * F;
    mat[5]  = -BD * F + A * E;
    mat[6]  =  -B * C;
    mat[8]  = -AD * E + B * F;
    mat[9]  =  AD * F + B * E;
    mat[10] =   A * C;
    mat[3]  =  mat[7] = mat[11] = mat[12] = mat[13] = mat[14] = 0;
    mat[15] =  1;

  Using basic matrix calculations, the operation count would reach<br>
  128 multiplications, 96 additions and  80 assignments operations.<br>
  Using the optimised algorithm, only 12 multiplications, 6 subtractions<br>
  and 18 assignment operations are required.<br>
  So, it is obvious that by using the optimised algorithm, a performance<br>
  achievement of 1000% is achieved!

<a name="Q37">Q37</a>. How do I convert a rotation matrix to Euler angles?
--------------------------------------------------------
  This operation is the exact opposite to the one answered in the question<br>
  above. Given that the rotation matrix is:

         |  CE      -CF       D   0 |
    M  = |  BDE+AF  -BDF+AE  -BC  0 |
         | -ADE+BF   ADF+BE   AC  0 |
         |  0        0        0   1 |

  where A,B are the cosine and sine of the X-axis rotation axis,<br>
        C,D are the cosine and sine of the Y-axis rotation axis,
        E,F are the cosine and sine of the Z-axis rotation axis.

  Using the C data structure for a 4x4 matrix, the index values are<br>
  as follows:

         |  0  1  2  3 |
    M =  |  4  5  6  7 |
         |  8  9 10 11 |
         | 12 13 14 15 |

  From looking at these two tables, it can be see that array element<br>
  [2] has the value of  D or  sin(Y). Then the rotation angle in the<br>
  Y-axis can be calculated from a call to to the inverse-sine function.<br>
  Passing this value to the cosine function then gives the value of C.

  If C is not zero, then the rotation angles in each of the X and Z<br>
  axii, can be derived from the terms on the third column and first row<br>
  respectively. These are as follows:

    X-axis:  M[6]  = -BC
             M[10] =  AC

    Z-axis:  M[0]  =  CE
             M[1]  = -CF

  The actual rotation angles can be derived by taking each pair of values<br>
  dividing by C and passing the results to the inverse tangent function.<br>
  If C is zero, then these calculations are not possible. In this case<br>
  the rotation angle in the Y-axis will be either -90 or +90. Thus D<br>
  will either have the value of 1 or -1.<br>
  In this case, Gimbal Lock will have occurred. Rotations in both the<br>
  X and Z axii will appear to be in the same axis. This can be seen<br>
  through the evaluation of the rotation axis.

         |  0.E       -0.F        1    0 |
    M  = |  B.1.E+AF  -B.1.F+AE  -B.0  0 |
         | -A.1.E+BF   A.1.F+BE   A.0  0 |
         |  0          0          0    1 |

  Multiplying out each term gives:

         |  0          0          1    0 |
    M  = |  BE+AF     -BF+AE      0    0 |
         | -AE+BF      AF+BE      0    0 |
         |  0          0          0    1 |

  Rearranging these terms gives:

         |   0          0          1    0 |
    M  = |   BE+AF      AE-BF      0    0 |
         | -(AE-BF)     BE+AF      0    0 |
         |   0          0          0    1 |

  Then it can be seen that the matrix is really of the form:

         |  0   0   1   0 |
    M  = |  V   W   0   0 |
         | -W   V   0   0 |
         |  0   0   0   1 |

  Where V has the value of BE+AF and<br>
        W has the value of AE-BF

  These two values can be considered to be the sin and cosine of a<br>
  single rotation axis.<br>
  The final algorithm is then as follows:

    angle_y = D =  asin( mat[2]);        /* Calculate Y-axis angle */
    C           =  cos( angle_y );
    angle_y    *=  RADIANS;
    if ( fabs( C ) > 0.005 )             /* Gimball lock? */
      {
      trx      =  mat[10] / C;           /* No, so get X-axis angle */
      try      = -mat[6]  / C;
      angle_x  = atan2( try, trx ) * RADIANS;
      trx      =  mat[0] / C;            /* Get Z-axis angle */
      try      = -mat[1] / C;
      angle_z  = atan2( try, trx ) * RADIANS;
      }
    else                                 /* Gimball lock has occurred */
      {
      angle_x  = 0;                      /* Set X-axis angle to zero */
      trx      =  mat[5];                 /* And calculate Z-axis angle */
      try      =  mat[4];
      angle_z  = atan2( try, trx ) * RADIANS;
      }

    /* return only positive angles in [0,360] */
    if (angle_x < 0) angle_x += 360;
    if (angle_y < 0) angle_y += 360;
    if (angle_z < 0) angle_z += 360;

<a name="Q38">Q38</a>. How do I generate a rotation matrix for a selected axis and angle?
-----------------------------------------------------------------------
  The simplest way to generate this type of rotation matrix is through the<br>
  use of quaternion mathematics.<br>
  See question [<a href="#Q53">Q53</a>: How do I convert a quaternion to a rotation matrix?]<br>
  for further details.<br>
  The following code snipped does most of the work (phi being the rotation<br>
  angle and (u,v,w) the rotation (axis) vector):

        rcos = cos(phi);
        rsin = sin(phi);
        matrix[0][0] =      rcos + u*u*(1-rcos);
        matrix[1][0] =  w * rsin + v*u*(1-rcos);
        matrix[2][0] = -v * rsin + w*u*(1-rcos);
        matrix[0][1] = -w * rsin + u*v*(1-rcos);
        matrix[1][1] =      rcos + v*v*(1-rcos);
        matrix[2][1] =  u * rsin + w*v*(1-rcos);
        matrix[0][2] =  v * rsin + u*w*(1-rcos);
        matrix[1][2] = -u * rsin + v*w*(1-rcos);
        matrix[2][2] =      rcos + w*w*(1-rcos);

  Don't forget to set the rest of the matrix to 0 (1 at [3][3]) if<br>
  you are using 4x4 matrices!

<a name="Q39">Q39</a>. How do I generate a rotation matrix to map one vector onto another?
------------------------------------------------------------------------
  When developing animation software, a common requirement is to find<br>
  a rotation matrix that will map one direction vector onto another.<br>
  This problem may be visualised by considering the two direction<br>
  vectors to be attached at their starting points. Then the entire<br>
  rotation space forms a unit sphere.<br>
  In theory, there are an infinite number of rotation axii and angles<br>
  that will map one vector onto the other. All of these axii lie on the<br>
  plane where all of the points are the exact same distance from both<br>
  vectors.<br>
  However, only one solution is of practical interest. This is the path<br>
  which covers the shortest angular distance between the two vectors.<br>
  The rotation axis to this path is calculated by taking the cross<br>
  product between the two vectors:

    Vaxis = Vs x Vf

  The rotation angle is calculated by taking the dot product between the<br>
  two vectors:

                -1
    Vangle = cos   ( Vs . Vf )

  One practical application of the solution to this problem is finding<br>
  the shortest flight path between two cities. In this case, each city<br>
  is represented as a direction vector generated from spherical<br>
  coordinates. Since planet Earth is spherical, the desired flight path<br>
  is the shortest angular rotation between the two cities.

  Note: If Vs and Vf are colinear, the cross product returns (0,0,0).<br>
  You should test for that case and use any of the 90 degree rotations<br>
  of either Vs or Vf as a rotation axis, e.g. (y,z,x). If x==y==z, then<br>
  using one of x,y, or z from the second vector might help.<br>
   --> Is there a better way?

  Having the rotation angle and vector, generating the corresponding matrix<br>
  is easy, see [<a href="#Q38">Q38</a>: How do I generate a rotation matrix for<br>
  a selected axis and angle?] for details.

  Don't let the spectre of Gimbal Lock fool you: Euler angles are still<br>
  a complete representation of any rotation in 3D space; it's just that<br>
  the actual Euler angles needed to achieve some particular desired<br>
  rotation may be rather unintuitive.

<a name="Q40">Q40</a>. How do I use matrices to convert one coordinate system to another?
-----------------------------------------------------------------------
  Similar to the previous problem, the requirement is to map one<br>
  coordinate system onto another. However, instead of just trying to<br>
  map one coordinate axis onto another, all three axii have to be matched.<br>
  Both coordinate systems are therefore represented as either 3x3 or<br>
  4x4 matrices.

  The problem is therefore to find the rotation matrix that will map one<br>
  matrix onto another. This can be expressed mathematically:

    Mfinal = Mrot . Morig

  where Mfinal is the final coordinate system matrix,<br>
        Morig  is the original coordinate system and
        Mrot   is the desired rotation matrix.

  The goal is then to find the matrix Mrot. This can be achieved by<br>
  rearranging the equation to give:

                  -1
    Mfinal . Morig   = Mrot

                           -1
    Mrot   = Mfinal . Morig

  Thus, the desired rotation matrix can be by calculatng the inverse of<br>
  the original coordinate system and multiplying it with the final<br>
  rotation matrix.

  As a check, consider the cases when either the original or final<br>
  rotation matrices are the identity matrix. In each case, the rotation<br>
  matrix should match the final matrix and the inverse of the final<br>
  matrix respectively.

  Once calculated, the rotation matrix may be converted into a<br>
  quaternion.

<a name="Q41">Q41</a>. What is a translation matrix?
----------------------------------
  A translation matrix is used to position an object within 3D space<br>
  without rotating in any way. Translation operations using matrix<br>
  multiplication can only be performed using 4x4 matrices.

  If the translation is defined by the vector [X Y Z ], then the 4x4<br>
  matrix to implement translation is as follows:

        | 1  0  0  X |
        |            |
        | 0  1  0  Y |
    M = |            |
        | 0  0  1  Z |
        |            |
        | 0  0  0  1 |

  If the vector is [0 0 0] then the vertex list will remain as before.

<a name="Q42">Q42</a>. What is a scaling matrix?
------------------------------
  A scaling matrix is used to enlarge or shrink the size of a 3D model.<br>
  If the scaling vector is [X Y Z] then the matrix to perform this is<br>
  as follows:

        | X  0  0  0 |
        |            |
        | 0  Y  0  0 |
    M = |            |
        | 0  0  Z  0 |
        |            |
        | 0  0  0  1 |

  If the scaling vector is [1 1 1], then this generates the identity<br>
  matrix and vertex geometry will remain unchanged.

<a name="Q43">Q43</a>. What is a shearing matrix?
-------------------------------
  A shearing matrix is used to make a 3D model appear to slant sideways.<br>
  For example, "italic" text requires each character to slant towards the<br>
  right.<br>
  In three dimensions six possible shearing directions exist:

  * shear X by Y
  * shear X by Z
  * shear Y by X
  * shear Y by Z
  * shear Z by X
  * shear Z by Y

  All six shearing directions may be combined into a single matrix:

        | 1    Syx  Szx  0 |
        |                  |
        | Sxy  1    Szy  0 |
    M = |                  |
        | Sxz  Syz  1    0 |
        |                  |
        | 0    0    0    1 |
        |                  |

    Where Sij implements a shear of I by J
    Thus, Sxy shears X by Y

  In theory, rotation in three dimensions may be considered a combination<br>
  of six shearing directions.

<a name="Q44">Q44</a>. How do I perform linear interpolation between two matrices?
----------------------------------------------------------------
  Given two rotation matrices, the problem is to find a way of<br>
  determining intermediate positions specified by a parametric<br>
  variable t, where t ranges from 0.0 to 1.0<br>
  This can be achieved by converting the two matrices into either<br>
  Euler angles or Spherical rotation angles (via quaternions) and<br>
  a translation vector.

  In either case, each matrix is converted into a pair of 3D vectors.<br>
  Interpolation between these two vectors can then be performed<br>
  through the use of the standard linear interpolation equation:

    Vr = Va + t .(Vb - Va )

  where Vr is the resulting vector<br>
        Va is the start position vector
        Vb is the final position vector

  This equation may be applied to both translation and rotation vectors.<br>
  Once determined, the resulting translation and rotation are then<br>
  converted back into the desired intermediate matrix.

<a name="Q45">Q45</a>. How do I perform cubic interpolation between four matrices?
----------------------------------------------------------------
  Given four rotation or translation matrices, the problem is to<br>
  find a way  of determining intermediate positions specified by a<br>
  parametric variable t.

  This can be achieved by making use of cubic interpolation. As with<br>
  linear interpolation, the four matrices are converted into their<br>
  corresponding translation and rotation vectors (Again, either Euler<br>
  angles or spherical rotation angles).

  Each set of four vectors is then converted into a single geometry<br>
  vector G. Through the use of spline mathematics, this geometry vector<br>
  is converted into an interpolation matrix M.

  If the geometry vector is defined as:

        | x1 x2 x3 x4 |
    G = | y1 y2 y3 y4 |
        | z1 z2 z3 z4 |

  Then multiplication by the base matrix:

         |  -4.5    9.0  -5.5  1.0  |
    Mb = |  13.5  -22.5   9.0  0.0  |
         | -13.5   18.0  -4.5  0.0  |
         |   4.5   -4.5   1.0  0.0  |

  will generate the 3x4 interpolation matrix Mi:

    Mi = G .Mb

  This can be implemented through a standard matrix-vector multiplication.<br>
  Interpolation can then be performed by the use of the parametric<br>
  variable t:

        R  = Mi . t

                           |t^3|
    | xr |   | A B C D |   |t^2|
    | yr | = | E F G H | . |t  |
    | zr |   | I J K L |   |1  |

  The result vector can then be converted back into a rotation or<br>
  translation matrix.

  It should be noted that the rotation paths that are generated may<br>
  occasionally become rather loopy. This is normal, as the algorithm<br>
  is trying to find the path with the least amount of rotation between<br>
  all four vectors.

  Of the two methods, spherical rotation angles will usually be seen to<br>
  provide the cleanest interpolation paths for rotation.

<a name="Q46">Q46</a>. How can I render a matrix?
-------------------------------
  When using a graphics window for 3D animation, it is convenient to be<br>
  able to view a rotation matrix concurrently with the animation.<br>
  However, displaying a rotation matrix as an array of numeric values<br>
  does not provide a very meaningful context.<br>
  An alternative to rendering numeric data is to make use of graphical<br>
  display methods such as bar-graphs.

  Much like a graphic equalizer on a stereo, a rotation matrix may be<br>
  displayed in a bar graph format. Each element of the rotation matrix<br>
  is rendered as an individual bar-graph in the range -1 to +1.<br>
  A 3x3 matrix would look like the following:

    +--+ +--+ +--+
    |##| |  | |  |
    +--+ +--+ +--+
    |  | |  | |  |
    +--+ +--+ +--+

    +--+ +--+ +--+
    |  | |##| |  |
    +--+ +--+ +--+
    |  | |  | |  |
    +--+ +--+ +--+

    +--+ +--+ +--+
    |  | |  | |##|
    +--+ +--+ +--+
    |  | |  | |  |
    +--+ +--+ +--+

  In this case, the rotation matrix is the identity matrix, since each<br>
  element in the major diagonal is +1, and all others are zero.<br>
  For added visual clarity, parameters which are negative may shaded<br>
  in a different colour than those which are positive.

QUATERNIONS
===========

<a name="Q47">Q47</a>. What are quaternions?
--------------------------
  Quaternions extend the concept of rotation in three dimensions to<br>
  rotation in four dimensions. This avoids the problem of "gimbal-lock"<br>
  and allows for the implementation of smooth and continuous rotation.<br>
  In effect, they may be considered to add a additional rotation angle<br>
  to spherical coordinates ie. Longitude, Latitude and Rotation angles<br>
  A Quaternion is defined using four floating point values |x y z w|.<br>
  These are calculated from the combination of the three coordinates<br>
  of the rotation axis and the rotation angle.

<a name="Q48">Q48</a>. How do quaternions relate to 3D animation?
-----------------------------------------------
  As mentioned before, Euler angles have the disadvantage of being<br>
  susceptible to "Gimbal lock" where attempts to rotate an<br>
  object fail to appear as expected, due to the order in which the<br>
  rotations are performed.

  Quaternions are a solution to this problem. Instead of rotating an<br>
  object through a series of successive rotations, quaternions allow<br>
  the programmer to rotate an object through an arbitary rotation axis<br>
  and angle.

  The rotation is still performed using matrix mathematics. However,<br>
  instead of multiplying matrices together, quaternions representing<br>
  the axii of rotation are multiplied together. The final resulting<br>
  quaternion is then converted to the desired rotation matrix.<br>
  Because the rotation axis is specifed as a unit direction vector,<br>
  it may also be calculated through vector mathematics or from<br>
  spherical coordinates ie (longitude/latitude).<br>
  Quaternions offer another advantage in that they be interpolated.<br>
  This allows for smooth and predictable rotation effects.

<a name="Q49">Q49</a>. How do I calculate the conjugate of a quaternion?
------------------------------------------------------
  This can be achieved by reversing the polarity (or negating) the<br>
  vector part of the quaternion, ie:

    Qr =  ( Qr.scalar, -Qr.vector )
  <br>

    quaternion_conjugate( QUAT *qr, QUAT *qa )
    {
      qr -> qw =  qa -> qw;
      qr -> qx = -qa -> qx;
      qr -> qy = -qa -> qy;
      qr -> qz = -qa -> qz;
    }

<a name="Q50">Q50</a>. How do I calculate the inverse of a quaternion?
----------------------------------------------------
  This is equivalent to calculating the conjugate of the quaternion,<br>
  if the quaternion is normalized (or a unit quaternion).<br>
  In all other cases, the magnitude of the inverse is 1/|q|.<br>
  See <a href="#Q49">Q49</a>: How do I calculate the conjugate of a quaternion?

<a name="Q51">Q51</a>. How do I calculate the magnitude of a quaternion?
------------------------------------------------------
  The magnitude of a quaternion is calculated by multiplying the<br>
  quaternion with its conjugate ie:<br>

               ------------
              /       --
    |Qr| =  \/     Qr.Qr

  This can be implemented as the following code sequence:<br>

    QFLOAT quaternion_magnitude( QUAT *qa )
    {
    return( sqrt(qa->qw*qa->qw+
                 qa->qx*qa->qx+ qa->qy*qa->qy+qa->qz*qa->qz) )
    }

<a name="Q52">Q52</a>. How do I normalise a quaternion?
-------------------------------------
  A quaternion can be normalised in a way similar to vectors. The<br>
  magnitude of the quaternion is calculated first. Then both the<br>
  scalar and vector part of the quaternion are divided by this value.<br>
  A unit quaternion will always have a magnitude of 1.0

<a name="Q53">Q53</a>. How do I multiply two quaternions together?
------------------------------------------------
  Given two quaternions Q1 and Q2, the goal is to calculate the<br>
  combined rotation Qr:

    Qr = Q1.Q2

  This is achieved through the expression:

    Qr = Q1.Q2 = ( w1.w2 - v1.v2, w1.v2 + w2.v1 + v1 x v2 )

  where v1 = (x,y,z) of Q1<br>
        w1 = (w)     of Q1
        v2 = (x,y,z) of Q2
        w2 = (w)     of Q2

  and both . and x are the standard vector dot and cross products.<br>
  This can be implemented using the following code segment:<br>

    quaternion_multiply( QUAT *qr, QUAT *qa, QUAT *qb )
    {
      qr.scalar = qa->scalar * qb->scalar - v3_dot( &qa->vector, &qb->vector );
      v3_cross(  &va, &qa->vector, &qb->vector );
      v3_scalef( &vb, &qa->vector, &qb->scalar );
      v3_scalef( &vc, &qb->vector, &qa->scalar );
      v3_add(    &va,         &va, &vb );
      v3_add(    &qr->vector, &va, &vc );
      quaternion_normalise( qr );
    }

  An optimization can also be made by rearranging to<br>

    w = w1w2 - x1x2 - y1y2 - z1z2
    x = w1x2 + x1w2 + y1z2 - z1y2
    y = w1y2 + y1w2 + z1x2 - x1z2
    z = w1z2 + z1w2 + x1y2 - y1x2

<a name="Q54">Q54</a>. How do I convert a quaternion to a rotation matrix?
--------------------------------------------------------
  Assuming that a quaternion has been created in the form:

    Q = |X Y Z W|

  Then the quaternion can then be converted into a 4x4 rotation<br>
  matrix using the following expression (Warning: you might have to<br>
  transpose this matrix if you (do not) follow the OpenGL order!):

         |        2     2                                      |
         | 1 - (2Y  + 2Z )   2XY + 2ZW         2XZ - 2YW       |
         |                                                     |
         |                          2     2                    |
     M = | 2XY - 2ZW         1 - (2X  + 2Z )   2YZ + 2XW       |
         |                                                     |
         |                                            2     2  |
         | 2XZ + 2YW         2YZ - 2XW         1 - (2X  + 2Y ) |
         |                                                     |

  If a 4x4 matrix is required, then the bottom row and right-most column<br>
  may be added.<br>
  The matrix may be generated using the following expression:

    xx      = X * X;
    xy      = X * Y;
    xz      = X * Z;
    xw      = X * W;
    yy      = Y * Y;
    yz      = Y * Z;
    yw      = Y * W;
    zz      = Z * Z;
    zw      = Z * W;
    mat[0]  = 1 - 2 * ( yy + zz );
    mat[1]  =     2 * ( xy - zw );
    mat[2]  =     2 * ( xz + yw );
    mat[4]  =     2 * ( xy + zw );
    mat[5]  = 1 - 2 * ( xx + zz );
    mat[6]  =     2 * ( yz - xw );
    mat[8]  =     2 * ( xz - yw );
    mat[9]  =     2 * ( yz + xw );
    mat[10] = 1 - 2 * ( xx + yy );
    mat[3]  = mat[7] = mat[11] = mat[12] = mat[13] = mat[14] = 0;
    mat[15] = 1;

  The resulting matrix uses the following positions:

        | mat[0]  mat[4] mat[ 8] mat[12] |
    M = | mat[1]  mat[5] mat[ 9] mat[13] |
        | mat[2]  mat[6] mat[10] mat[14] |
        | mat[3]  mat[7] mat[11] mat[15] |

<a name="Q55">Q55</a>. How do I convert a rotation matrix to a quaternion?
--------------------------------------------------------
  A rotation may be converted back to a quaternion through the use of<br>
  the following algorithm:<br>
  The process is performed in the following stages, which are as follows:

    Calculate the trace of the matrix T from the equation:

                2     2     2
      T = 4 - 4x  - 4y  - 4z

                 2    2    2
        = 4( 1 -x  - y  - z )

        = 1 + mat[0] + mat[5] + mat[10]


    If the trace of the matrix is greater than zero, then
    perform an "instant" calculation.
    Important note wrt. rouning errors:

    Test if ( T > 0.00000001 ) to avoid large distortions!

      S = sqrt(T) * 2;
      X = ( mat[9] - mat[6] ) / S;
      Y = ( mat[2] - mat[8] ) / S;
      Z = ( mat[4] - mat[1] ) / S;
      W = 0.25 * S;

    If the trace of the matrix is equal to zero then identify
    which major diagonal element has the greatest value.
    Depending on this, calculate the following:

    if ( mat[0] > mat[5] && mat[0] > mat[10] )  {        // Column 0:
        S  = sqrt( 1.0 + mat[0] - mat[5] - mat[10] ) * 2;
        X = 0.25 * S;
        Y = (mat[4] + mat[1] ) / S;
        Z = (mat[2] + mat[8] ) / S;
        W = (mat[9] - mat[6] ) / S;
    } else if ( mat[5] > mat[10] ) {                        // Column 1:
        S  = sqrt( 1.0 + mat[5] - mat[0] - mat[10] ) * 2;
        X = (mat[4] + mat[1] ) / S;
        Y = 0.25 * S;
        Z = (mat[9] + mat[6] ) / S;
        W = (mat[2] - mat[8] ) / S;
    } else {                                                // Column 2:
        S  = sqrt( 1.0 + mat[10] - mat[0] - mat[5] ) * 2;
        X = (mat[2] + mat[8] ) / S;
        Y = (mat[9] + mat[6] ) / S;
        Z = 0.25 * S;
        W = (mat[4] - mat[1] ) / S;
    }

     The quaternion is then defined as:
       Q = | X Y Z W |

<a name="Q56">Q56</a>. How do I convert a rotation axis and angle to a quaternion?
----------------------------------------------------------------
  Given a rotation axis and angle, the following<br>
  algorithm may be used to generate a quaternion:

    vector_normalize(axis);
    sin_a = sin( angle / 2 );
    cos_a = cos( angle / 2 );
    X    = axis -> x * sin_a;
    Y    = axis -> y * sin_a;
    Z    = axis -> z * sin_a;
    W    = cos_a;

  It is necessary to normalise the quaternion in case any values are<br>
  very close to zero.

<a name="Q57">Q57</a>. How do I convert a quaternion to a rotation axis and angle?
----------------------------------------------------------------
  A quaternion can be converted back to a rotation axis and angle<br>
  using the following algorithm:

    quaternion_normalise( |X,Y,Z,W| );
    cos_a = W;
    angle = acos( cos_a ) * 2;
    sin_a = sqrt( 1.0 - cos_a * cos_a );
    if ( fabs( sin_a ) < 0.0005 ) sin_a = 1;
    axis -> x = X / sin_a;
    axis -> y = Y / sin_a;
    axis -> z = Z / sin_a;

<a name="Q58">Q58</a>. How do I convert spherical rotation angles to a quaternion?
----------------------------------------------------------------
  A rotation axis itself may be defined using spherical coordinates<br>
  (latitude and longitude) and a rotation angle<br>
  In this case, the quaternion can be calculated as follows:

    sin_a    = sin( angle / 2 )
    cos_a    = cos( angle / 2 )
    sin_lat  = sin( latitude )
    cos_lat  = cos( latitude )
    sin_long = sin( longitude )
    cos_long = cos( longitude )
    X       = sin_a * cos_lat * sin_long
    Y       = sin_a * sin_lat
    Z       = sin_a * sin_lat * cos_long
    W       = cos_a

  WARNING: There might be a problem in this code.<br>
  An alternative is the code snipped given in [<a href="#Q60">Q60</a>: How<br>
  do I convert Euler rotation angles to a quaternion?"].

<a name="Q59">Q59</a>. How do I convert a quaternion to spherical rotation angles?
----------------------------------------------------------------
  A quaternion can be converted to spherical coordinates by extending<br>
  the conversion process:

    cos_a  = W;
    sin_a  = sqrt( 1.0 - cos_a * cos_a );
    angle  = acos( cos_a ) * 2;
    if ( fabs( sin_angle ) < 0.0005 ) sin_a = 1;
    tx = X / sin_a;
    ty = Y / sin_a;
    tz = Z / sin_a;
    latitude = -asin( ty );
    if ( tx * tx + tz * tz < 0.0005 )
      longitude   = 0;
    else
       longitude  = atan2( tx, tz );
    if ( longitude < 0 )
      longitude += 360.0;

  WARNING: In this code might still be a problem.<br>
  Please let me know what it is and how to fix this.

<a name="Q60">Q60</a>. How do I convert Euler rotation angles to a quaternion?
-------------------------------------------------------------------
  Converting Euler rotation angles to quaterions can be achieved through<br>
  the use of quaternion multiplication. Each rotation angle is converted<br>
  to an axis-angle pair, with the axis corresponding to one of the<br>
  Euclidean axii. The axis-angle pairs are converted to quaternions and<br>
  multiplied together. The final quaternion is the desired result.


  The following code segment demonstrates this:

    quaternion_from_euler( QUATERNION *q, VFLOAT ax, VFLOAT ay, VFLOAT az )
    {
      VECTOR3 vx = { 1, 0, 0 }, vy = { 0, 1, 0 }, vz = { 0, 0, 1 };
      QUATERNION qx, qy, qz, qt;
      quaternion_from_axisangle( qx, &vx, rx );
      quaternion_from_axisangle( qy, &vy, ry );
      quaternion_from_axisangle( qz, &vz, rz );
      quaternion_multiply( &qt, &qx, &qy );
      quaternion_multiply( &q,  &qt, &qz );
    }

  The following more or less comes from:<br>
  http://vered.rose.utoronto.ca/people/david_dir/GEMS/GEMS.html

    //Pitch->X axis, Yaw->Y axis, Roll->Z axis
    Quaternion::Quaternion(float fPitch, float fYaw, float fRoll)
    {
       const float fSinPitch(sin(fPitch*0.5F));
       const float fCosPitch(cos(fPitch*0.5F));
       const float fSinYaw(sin(fYaw*0.5F));
       const float fCosYaw(cos(fYaw*0.5F));
       const float fSinRoll(sin(fRoll*0.5F));
       const float fCosRoll(cos(fRoll*0.5F));
       const float fCosPitchCosYaw(fCosPitch*fCosYaw);
       const float fSinPitchSinYaw(fSinPitch*fSinYaw);
       X = fSinRoll * fCosPitchCosYaw     - fCosRoll * fSinPitchSinYaw;
       Y = fCosRoll * fSinPitch * fCosYaw + fSinRoll * fCosPitch * fSinYaw;
       Z = fCosRoll * fCosPitch * fSinYaw - fSinRoll * fSinPitch * fCosYaw;
       W = fCosRoll * fCosPitchCosYaw     + fSinRoll * fSinPitchSinYaw;
    }

  The following might also work:<br>

    QUATERNION qx = { cos(pitch/2f), sin(pitch/2f), 0, 0 }
    QUATERNION qy = { cos(yaw/2f), 0, sin(yaw/2f), 0 }
    QUATERNION qz = { cos(roll/2f), 0, 0, sin(roll/2f) }
    quaternion_multiply( &qt, &qx, &qy );
    quaternion_multiply( &q,  &qt, &qz );

  In Java looks like this:

    public static void setQ( Quat4f q, float pitch, float yaw, float roll )
    {
      Quat4f qx = new Quat4f((float) Math.cos(pitch/2f),
                             (float) Math.sin(pitch/2f), 0, 0);
      Quat4f qy = new Quat4f((float) Math.cos(yaw/2f), 0,
                             (float) Math.sin(yaw/2f),0);
      Quat4f qz = new Quat4f((float) Math.cos(roll/2f), 0, 0,
                             (float) Math.sin(roll/2f) );
      Quat4f qt = new Quat4f();
      qt.set( qx );
      qt.mul( qy );
      qt.mul( qz );
      q.set( qt );
    }

<a name="Q61">Q61</a>. How do I use quaternions to perform linear interpolation between matrices?
-------------------------------------------------------------------------------
  For many animation applications, it is necessary to interpolate<br>
  between two rotation positions of a given object. These positions may<br>
  have been specified using keyframe animation or inverse kinematics.<br>
  Using either method, at least two rotation matrices must be known, and<br>
  the desired goal is to interpolate between them. The two matrices are<br>
  referred to as the starting and finish matrices( MS and MF).<br>
  Using linear interpolation, the interpolated rotation matrix is<br>
  generated using a blending equation with the parameter T, which<br>
  ranges from 0.0 to 1.0.

  At T=0, the interpolated matrix is equal to the starting matrix.<br>
  At T=1, the interpolated matrix is equal to the finishing matrix.<br>
  Then the interpolated rotation matrix (MI) is specified as:

    MI = F( MS, MF, T )

  where F is a blending function.<br>
  The first stage in interpolating between the two matrices is to<br>
  determine the rotation matrix that will convert MS to MF.<br>
  This is achieved using the following expression:

          -1
    T = Ms  . Mf

  where Ms is the start matrix,<br>
        Mf is the finish matrix,
    and T is the intermediate matrix.

  The next stage is to convert this matrix into a rotation axis and<br>
  angle. This is achieved by converting the matrix into a quaternion<br>
  and finally into the required rotation axis and angle.<br>
  In order to generate the interpolated rotation matrix, it is only<br>
  necessary to scale the rotation angle and convert this angle and<br>
  the rotation axis back into a rotation matrix.

  Using a 4x4 matrix library, this is as follows:

    m4_transpose(    mt, ms );                /* Inverse             */
    m4_mult(         ms, mt, mb );            /* Rotation matrix     */
    m4_to_axisangle( ms, axis, angle );       /* Rotation axis/angle */
    for ( t = 0; t < 1.0; t += 0.05 )
      {
      m4_from_axisangle( mi, axis, angle * t ); /* Final interpolation */
      ... whatever ...
      }

  where t is the interpolation factor ranging from 0.0 to 1.0

<a name="Q62">Q62</a>. How do I use quaternions to perform cubic interpolation between matrices?
------------------------------------------------------------------------------
  For some applications, it may not be convenient or possible to use linear<br>
  interpolation for animation purposes. In this case, cubic interpolation<br>
  is another alternative.<br>
  In order to use cubic interpolation, at least four rotation matrices must<br>
  be known.

  Each of these is then converted into a set of spherical rotations<br>
  via quaternions and spherical rotation angles (ie. longitude, latitude<br>
  and rotation angle).

  These are then multiplied with the base matrix for a Cardinal spline<br>
  curve. This interpolation matrix can then be used to determine the<br>
  intermediate spherical rotation angles.<br>
  Once the interpolated coordinates are known (latitude, longitude and<br>
  rotation angle), the interpolated rotation matrix can then be generated<br>
  through the conversion to quaternions.

  Using a 4x4 matrix library, the algorithm is as follows:

    for ( n = 0; n < 4; n++ )
      m4_to_spherical( mat[n], &v_sph[n] );   /* Spherical coordinates */
    m4_multspline( m_cardinal, v_sph, v_interp ); /* Interpolation vector */
    ...
    v3_cubic( v_pos, v_interp, t );           /* Interpolation */
    m4_from_spherical( m_rot, v_pos );        /* Back to a matrix */

<a name="Q63">Q63</a>. How do I use quaternions to rotate a vector?
------------------------------------------------------------------------------
  A rather elegant way to rotate a vector using a quaternion directly<br>
  is the following (qr being the rotation quaternion):

                       -1
       v' = qr * v * qr

  This can easily be realised and is most likely faster then the transformation<br>
  using a rotation matrix.



<script language="Javascript"><br>
<!--

// FILE ARCHIVED ON 20041029003853 AND RETRIEVED FROM THE<br>
// INTERNET ARCHIVE ON 20050827150132.<br>
// JAVASCRIPT APPENDED BY WAYBACK MACHINE, COPYRIGHT INTERNET ARCHIVE.<br>
// ALL OTHER CONTENT MAY ALSO BE PROTECTED BY COPYRIGHT (17 U.S.C.<br>
// SECTION 108(a)(3)).

   var sWayBackCGI = "http://web.archive.org/web/20041029003853/";

   function xLateUrl(aCollection, sProp) {<br>
      var i = 0;
      for(i = 0; i < aCollection.length; i++)
         if (aCollection[i][sProp].indexOf("mailto:") == -1 &&
             aCollection[i][sProp].indexOf("javascript:") == -1)
            aCollection[i][sProp] = sWayBackCGI + aCollection[i][sProp];
   }

   if (document.links)  xLateUrl(document.links, "href");<br>
   if (document.images) xLateUrl(document.images, "src");<br>
   if (document.embeds) xLateUrl(document.embeds, "src");

   if (document.body && document.body.background)<br>
      document.body.background = sWayBackCGI + document.body.background;

//-->

</script><br>
</html>
